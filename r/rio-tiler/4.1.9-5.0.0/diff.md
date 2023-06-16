# Comparing `tmp/rio_tiler-4.1.9.tar.gz` & `tmp/rio_tiler-5.0.0.tar.gz`

## Comparing `rio_tiler-4.1.9.tar` & `rio_tiler-5.0.0.tar`

### file list

```diff
@@ -1,198 +1,197 @@
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/setup.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/__init__.py
--rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/colormap.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/constants.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/errors.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/expression.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/logger.py
--rw-r--r--   0        0        0    22175 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/models.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/profiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/py.typed
--rw-r--r--   0        0        0    19338 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/reader.py
--rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/tasks.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/types.py
--rw-r--r--   0        0        0    22537 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/utils.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/accent.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/accent_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/afmhot.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/afmhot_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/autumn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/autumn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/binary.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/binary_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/blues.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/blues_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/bone.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/bone_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/brbg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/brbg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/brg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/brg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/bugn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/bugn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/bupu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/bupu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/bwr.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/bwr_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/cfastie.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/cividis.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/cividis_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/cmrmap.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/cmrmap_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/cool.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/cool_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/coolwarm.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/coolwarm_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/copper.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/copper_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/cubehelix.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/cubehelix_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/dark2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/dark2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/flag.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/flag_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gist_earth.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gist_earth_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gist_gray.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gist_gray_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gist_heat.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gist_heat_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gist_ncar.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gist_ncar_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gist_rainbow.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gist_rainbow_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gist_stern.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gist_stern_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gist_yarg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gist_yarg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gnbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gnbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gnuplot.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gnuplot2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gnuplot2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gnuplot_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gray.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/gray_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/greens.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/greens_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/greys.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/greys_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/hot.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/hot_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/hsv.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/hsv_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/inferno.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/inferno_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/jet.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/jet_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/magma.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/magma_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/nipy_spectral.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/nipy_spectral_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/ocean.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/ocean_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/oranges.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/oranges_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/orrd.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/orrd_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/paired.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/paired_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/pastel1.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/pastel1_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/pastel2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/pastel2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/pink.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/pink_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/piyg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/piyg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/plasma.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/plasma_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/prgn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/prgn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/prism.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/prism_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/pubu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/pubu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/pubugn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/pubugn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/puor.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/puor_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/purd.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/purd_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/purples.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/purples_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/rainbow.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/rainbow_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/rdbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/rdbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/rdgy.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/rdgy_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/rdpu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/rdpu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/rdylbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/rdylbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/rdylgn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/rdylgn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/reds.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/reds_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/rplumbo.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/schwarzwald.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/seismic.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/seismic_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/set1.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/set1_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/set2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/set2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/set3.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/set3_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/spectral.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/spectral_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/spring.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/spring_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/summer.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/summer_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/tab10.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/tab10_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/tab20.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/tab20_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/tab20b.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/tab20b_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/tab20c.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/tab20c_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/terrain.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/terrain_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/twilight.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/twilight_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/twilight_shifted.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/twilight_shifted_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/viridis.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/viridis_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/winter.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/winter_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/wistia.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/wistia_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/ylgn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/ylgn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/ylgnbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/ylgnbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/ylorbr.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/ylorbr_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/ylorrd.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/cmap_data/ylorrd_r.npy
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/io/__init__.py
--rw-r--r--   0        0        0    41212 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/io/base.py
--rw-r--r--   0        0        0    31047 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/io/rasterio.py
--rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/io/stac.py
--rw-r--r--   0        0        0    14507 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/io/xarray.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/mosaic/__init__.py
--rw-r--r--   0        0        0     8314 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/mosaic/reader.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/mosaic/methods/__init__.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/mosaic/methods/base.py
--rw-r--r--   0        0        0     6651 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/rio_tiler/mosaic/methods/defaults.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/.gitignore
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/AUTHORS.txt
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/LICENSE
--rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/README.md
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/pyproject.toml
--rw-r--r--   0        0        0    11788 2020-02-02 00:00:00.000000 rio_tiler-4.1.9/PKG-INFO
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/__init__.py
+-rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/colormap.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/constants.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/errors.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/expression.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/logger.py
+-rw-r--r--   0        0        0    25431 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/models.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/profiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/py.typed
+-rw-r--r--   0        0        0    20985 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/reader.py
+-rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/tasks.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/types.py
+-rw-r--r--   0        0        0    21907 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/utils.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/accent.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/accent_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/afmhot.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/afmhot_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/autumn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/autumn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/binary.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/binary_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/blues.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/blues_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/bone.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/bone_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/brbg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/brbg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/brg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/brg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/bugn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/bugn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/bupu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/bupu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/bwr.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/bwr_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/cfastie.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/cividis.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/cividis_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/cmrmap.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/cmrmap_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/cool.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/cool_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/coolwarm.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/coolwarm_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/copper.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/copper_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/cubehelix.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/cubehelix_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/dark2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/dark2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/flag.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/flag_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gist_earth.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gist_earth_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gist_gray.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gist_gray_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gist_heat.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gist_heat_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gist_ncar.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gist_ncar_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gist_rainbow.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gist_rainbow_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gist_stern.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gist_stern_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gist_yarg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gist_yarg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gnbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gnbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gnuplot.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gnuplot2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gnuplot2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gnuplot_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gray.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/gray_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/greens.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/greens_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/greys.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/greys_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/hot.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/hot_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/hsv.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/hsv_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/inferno.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/inferno_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/jet.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/jet_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/magma.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/magma_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/nipy_spectral.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/nipy_spectral_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/ocean.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/ocean_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/oranges.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/oranges_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/orrd.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/orrd_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/paired.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/paired_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/pastel1.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/pastel1_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/pastel2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/pastel2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/pink.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/pink_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/piyg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/piyg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/plasma.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/plasma_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/prgn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/prgn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/prism.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/prism_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/pubu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/pubu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/pubugn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/pubugn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/puor.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/puor_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/purd.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/purd_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/purples.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/purples_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/rainbow.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/rainbow_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/rdbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/rdbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/rdgy.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/rdgy_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/rdpu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/rdpu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/rdylbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/rdylbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/rdylgn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/rdylgn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/reds.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/reds_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/rplumbo.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/schwarzwald.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/seismic.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/seismic_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/set1.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/set1_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/set2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/set2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/set3.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/set3_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/spectral.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/spectral_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/spring.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/spring_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/summer.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/summer_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/tab10.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/tab10_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/tab20.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/tab20_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/tab20b.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/tab20b_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/tab20c.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/tab20c_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/terrain.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/terrain_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/twilight.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/twilight_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/twilight_shifted.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/twilight_shifted_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/viridis.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/viridis_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/winter.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/winter_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/wistia.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/wistia_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/ylgn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/ylgn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/ylgnbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/ylgnbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/ylorbr.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/ylorbr_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/ylorrd.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/cmap_data/ylorrd_r.npy
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/io/__init__.py
+-rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/io/base.py
+-rw-r--r--   0        0        0    31879 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/io/rasterio.py
+-rw-r--r--   0        0        0    10091 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/io/stac.py
+-rw-r--r--   0        0        0    16046 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/io/xarray.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/mosaic/__init__.py
+-rw-r--r--   0        0        0     8111 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/mosaic/reader.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/mosaic/methods/__init__.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/mosaic/methods/base.py
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/rio_tiler/mosaic/methods/defaults.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/.gitignore
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/AUTHORS.txt
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/LICENSE
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/README.md
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 rio_tiler-5.0.0/PKG-INFO
```

### Comparing `rio_tiler-4.1.9/rio_tiler/colormap.py` & `rio_tiler-5.0.0/rio_tiler/colormap.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/errors.py` & `rio_tiler-5.0.0/rio_tiler/errors.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/expression.py` & `rio_tiler-5.0.0/rio_tiler/expression.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     return [expr for expr in expression.split(";") if expr]
 
 
 def apply_expression(
     blocks: Sequence[str],
     bands: Sequence[str],
     data: numpy.ndarray,
-) -> numpy.ndarray:
+) -> numpy.ma.MaskedArray:
     """Apply rio-tiler expression.
 
     Args:
 
         blocks (sequence): expression for a specific layer.
         bands (sequence): bands names.
         data (numpy.array):  array of bands.
@@ -64,15 +64,15 @@
 
     """
     if len(bands) != data.shape[0]:
         raise ValueError(
             f"Incompatible number of bands ({bands}) and data shape {data.shape}"
         )
 
-    return numpy.array(
+    return numpy.ma.MaskedArray(
         [
             numpy.nan_to_num(
                 numexpr.evaluate(bloc.strip(), local_dict=dict(zip(bands, data)))
             )
             for bloc in blocks
             if bloc
         ]
```

### Comparing `rio_tiler-4.1.9/rio_tiler/models.py` & `rio_tiler-5.0.0/rio_tiler/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,23 +10,30 @@
 from affine import Affine
 from color_operations import parse_operations, scale_dtype, to_math_type
 from pydantic import BaseModel
 from rasterio import windows
 from rasterio.coords import BoundingBox
 from rasterio.crs import CRS
 from rasterio.dtypes import dtype_ranges
-from rasterio.enums import ColorInterp, Resampling
+from rasterio.enums import ColorInterp
 from rasterio.io import MemoryFile
 from rasterio.plot import reshape_as_image
 from rasterio.transform import from_bounds
 
 from rio_tiler.colormap import apply_cmap
 from rio_tiler.errors import InvalidDatatypeWarning, InvalidPointDataError
 from rio_tiler.expression import apply_expression, get_expression_blocks
-from rio_tiler.types import BBox, ColorMapType, GDALColorMapType, IntervalTuple, NumType
+from rio_tiler.types import (
+    BBox,
+    ColorMapType,
+    GDALColorMapType,
+    IntervalTuple,
+    NumType,
+    RIOResampling,
+)
 from rio_tiler.utils import (
     get_array_statistics,
     linear_rescale,
     non_alpha_indexes,
     render,
     resize_array,
 )
@@ -108,66 +115,79 @@
 
 def to_coordsbbox(bbox) -> Optional[BoundingBox]:
     """Convert bbox to CoordsBbox nameTuple."""
     return BoundingBox(*bbox) if bbox else None
 
 
 def rescale_image(
-    data: numpy.ndarray,
-    mask: numpy.ndarray,
+    array: numpy.ma.MaskedArray,
     in_range: Sequence[IntervalTuple],
     out_range: Sequence[IntervalTuple] = ((0, 255),),
     out_dtype: Union[str, numpy.number] = "uint8",
-):
-    """Rescale image data."""
-    if len(data.shape) < 3:
-        data = numpy.expand_dims(data, axis=0)
+) -> numpy.ma.MaskedArray:
+    """Rescale image data in-place."""
+    if len(array.shape) < 3:
+        array = numpy.expand_dims(array, axis=0)
 
-    nbands = data.shape[0]
+    nbands = array.shape[0]
 
     if len(in_range) != nbands:
         in_range = ((in_range[0]),) * nbands
 
     if len(out_range) != nbands:
         out_range = ((out_range[0]),) * nbands
 
     for bdx in range(nbands):
-        data[bdx] = numpy.where(
-            mask,
-            linear_rescale(data[bdx], in_range=in_range[bdx], out_range=out_range[bdx]),
+        array.data[bdx] = numpy.where(
+            ~array.mask[bdx],
+            linear_rescale(
+                array.data[bdx], in_range=in_range[bdx], out_range=out_range[bdx]
+            ),
             0,
         )
 
-    return data.astype(out_dtype)
+    return array.astype(out_dtype)
+
+
+def to_masked(array: numpy.ndarray) -> numpy.ma.MaskedArray:
+    """Makes sure we have a MaskedArray."""
+    if not numpy.ma.isarray(array):
+        array = numpy.ma.asarray(array)
+
+    # when a masked array is totally valid, the mask is set to numpy.ma.nomask
+    # https://numpy.org/doc/stable/reference/maskedarray.baseclass.html#numpy.ma.nomask
+    # doing `array.mask = False` force the creation of the mask array
+    if not array.mask.shape:
+        array.mask = False
+
+    return array
 
 
 @attr.s
 class PointData:
     """Point Data class.
 
     Attributes:
-        data (numpy.ndarray): pixel values.
-        mask (numpy.ndarray): rasterio mask values.
+        array (numpy.ma.MaskedArray): pixel values.
         band_names (list): name of each band. Defaults to `["1", "2", "3"]` for 3 bands image.
         coordinates (tuple): Point's coordinates.
         crs (rasterio.crs.CRS, optional): Coordinates Reference System of the bounds.
         assets (list, optional): list of assets used to construct the data values.
         metadata (dict, optional): Additional metadata. Defaults to `{}`.
 
     """
 
-    data: numpy.ndarray = attr.ib()
-    mask: numpy.ndarray = attr.ib()
-    band_names: List[str] = attr.ib()
-    coordinates: Optional[Tuple[float, float]] = attr.ib(default=None)
-    crs: Optional[CRS] = attr.ib(default=None)
-    assets: Optional[List] = attr.ib(default=None)
-    metadata: Optional[Dict] = attr.ib(factory=dict)
+    array: numpy.ma.MaskedArray = attr.ib(converter=to_masked)
+    band_names: List[str] = attr.ib(kw_only=True)
+    coordinates: Optional[Tuple[float, float]] = attr.ib(default=None, kw_only=True)
+    crs: Optional[CRS] = attr.ib(default=None, kw_only=True)
+    assets: Optional[List] = attr.ib(default=None, kw_only=True)
+    metadata: Optional[Dict] = attr.ib(factory=dict, kw_only=True)
 
-    @data.validator
+    @array.validator
     def _validate_data(self, attribute, value):
         """PointsData data has to be a 1d array."""
         if not len(value.shape) == 1:
             raise ValueError("PointsData data has to be a 1D array")
 
     @coordinates.validator
     def _validate_coordinates(self, attribute, value):
@@ -175,27 +195,39 @@
         if value and not len(value) == 2:
             raise ValueError("Coordinates data has to be a 2d list")
 
     @band_names.default
     def _default_names(self):
         return [f"b{ix + 1}" for ix in range(self.count)]
 
-    @mask.default
-    def _default_mask(self):
-        return numpy.array([255], dtype="uint8")
+    ###########################################################################
+    # For compatibility
+    @property
+    def data(self) -> numpy.ndarray:
+        """Return data part of the masked array."""
+        return self.array.data
+
+    @property
+    def mask(self) -> numpy.ndarray:
+        """Return Mask in form of rasterio dataset mask."""
+        return numpy.array([numpy.logical_and.reduce(~self.array.mask)]) * numpy.uint8(
+            255
+        )
+
+    ###########################################################################
 
     def __iter__(self):
         """Allow for variable expansion."""
-        for i in self.data:
+        for i in self.array.data:
             yield i
 
     @property
     def count(self) -> int:
         """Number of band."""
-        return self.data.shape[0]
+        return self.array.shape[0]
 
     @classmethod
     def create_from_list(cls, data: Sequence["PointData"]):
         """Create PointData from a sequence of PointsData objects.
 
         Args:
             data (sequence): sequence of PointData.
@@ -208,122 +240,153 @@
         if all([pt.coordinates or pt.crs or None for pt in data]):
             lon, lat, crs = zip(*[(*(pt.coordinates or []), pt.crs) for pt in data])
             if len(set(lon)) > 1 or len(set(lat)) > 1 or len(set(crs)) > 1:
                 raise InvalidPointDataError(
                     "Cannot concatenate points with different coordinates/CRS."
                 )
 
-        arr = numpy.concatenate([pt.data for pt in data])
-        mask = numpy.concatenate([pt.mask for pt in data]).all() * numpy.array(
-            [255], dtype="uint8"
-        )
+        arr = numpy.ma.concatenate([pt.array for pt in data])
 
         assets = list(
             dict.fromkeys(
                 itertools.chain.from_iterable([pt.assets for pt in data if pt.assets])
             )
         )
 
         band_names = list(
             itertools.chain.from_iterable(
                 [pt.band_names for pt in data if pt.band_names]
             )
         )
 
+        metadata = dict(
+            itertools.chain.from_iterable(
+                [pt.metadata.items() for pt in data if pt.metadata]
+            )
+        )
+
         return cls(
             arr,
-            mask,
             assets=assets,
             crs=data[0].crs,
             coordinates=data[0].coordinates,
             band_names=band_names,
+            metadata=metadata,
         )
 
     def as_masked(self) -> numpy.ma.MaskedArray:
         """return a numpy masked array."""
-        data = numpy.ma.array(self.data)
-        data.mask = self.mask == 0
-        return data
+        warnings.warn(
+            "'PointData.as_masked' has been deprecated and will be removed"
+            "in rio-tiler 6.0. You can get the masked array directly with `PointData.array` attribute.",
+            DeprecationWarning,
+        )
+        return self.array
 
     def apply_expression(self, expression: str) -> "PointData":
         """Apply expression to the image data."""
         blocks = get_expression_blocks(expression)
+
+        data = apply_expression(blocks, self.band_names, self.array)
+        # Using numexpr do not preserve mask info
+        data.mask = False
+
         return PointData(
-            apply_expression(blocks, self.band_names, self.data),
-            self.mask,
+            data,
             assets=self.assets,
             crs=self.crs,
             coordinates=self.coordinates,
             band_names=blocks,
             metadata=self.metadata,
         )
 
 
-def to_3d(data: numpy.ndarray) -> numpy.ndarray:
-    """Makes sure we have a 3D array."""
-    if len(data.shape) < 3:
-        data = numpy.expand_dims(data, axis=0)
+def masked_and_3d(array: numpy.ndarray) -> numpy.ma.MaskedArray:
+    """Makes sure we have a 3D array and mask"""
+    if not numpy.ma.isarray(array):
+        array = numpy.ma.asarray(array)
+
+    if len(array.shape) < 3:
+        array = numpy.expand_dims(array, axis=0)
+
+    # when a masked array is totally valid, the mask is set to numpy.ma.nomask
+    # https://numpy.org/doc/stable/reference/maskedarray.baseclass.html#numpy.ma.nomask
+    # doing `array.mask = False` force the creation of the mask array
+    if not array.mask.shape:
+        array.mask = False
 
-    return data
+    return array
 
 
 @attr.s
 class ImageData:
     """Image Data class.
 
     Attributes:
-        data (numpy.ndarray): pixel values.
-        mask (numpy.ndarray): rasterio mask values.
+        array (numpy.ma.MaskedArray): image values.
         assets (list, optional): list of assets used to construct the data values.
         bounds (BoundingBox, optional): bounding box of the data.
         crs (rasterio.crs.CRS, optional): Coordinates Reference System of the bounds.
         metadata (dict, optional): Additional metadata. Defaults to `{}`.
         band_names (list, optional): name of each band. Defaults to `["1", "2", "3"]` for 3 bands image.
         dataset_statistics (list, optional): dataset statistics `[(min, max), (min, max)]`
 
+    Note: `mask` should be considered as `PER_BAND` so shape should be similar as the data
+
     """
 
-    data: numpy.ndarray = attr.ib(converter=to_3d)
-    mask: numpy.ndarray = attr.ib()
-    assets: Optional[List] = attr.ib(default=None)
-    bounds: Optional[BoundingBox] = attr.ib(default=None, converter=to_coordsbbox)
-    crs: Optional[CRS] = attr.ib(default=None)
-    metadata: Optional[Dict] = attr.ib(factory=dict)
-    band_names: List[str] = attr.ib()
-    dataset_statistics: Optional[Sequence[Tuple[float, float]]] = attr.ib(default=None)
+    array: numpy.ma.MaskedArray = attr.ib(converter=masked_and_3d)
+    assets: Optional[List] = attr.ib(default=None, kw_only=True)
+    bounds: Optional[BoundingBox] = attr.ib(
+        default=None, converter=to_coordsbbox, kw_only=True
+    )
+    crs: Optional[CRS] = attr.ib(default=None, kw_only=True)
+    metadata: Optional[Dict] = attr.ib(factory=dict, kw_only=True)
+    band_names: List[str] = attr.ib(kw_only=True)
+    dataset_statistics: Optional[Sequence[Tuple[float, float]]] = attr.ib(
+        default=None, kw_only=True
+    )
+    cutline_mask: Optional[numpy.ndarray] = attr.ib(default=None)
 
     @band_names.default
     def _default_names(self):
         return [f"b{ix + 1}" for ix in range(self.count)]
 
-    @mask.default
-    def _default_mask(self):
-        return numpy.zeros((self.height, self.width), dtype="uint8") + 255
+    ###########################################################################
+    # For compatibility
+    @property
+    def data(self) -> numpy.ndarray:
+        """Return data part of the masked array."""
+        return self.array.data
+
+    @property
+    def mask(self) -> numpy.ndarray:
+        """Return Mask in form of rasterio dataset mask."""
+        return numpy.logical_or.reduce(~self.array.mask) * numpy.uint8(255)
+
+    ###########################################################################
 
     def __iter__(self):
         """Allow for variable expansion (``arr, mask = ImageData``)"""
-        for i in (self.data, self.mask):
+        for i in (self.array.data, self.mask):
             yield i
 
     @classmethod
     def from_array(cls, arr: numpy.ndarray) -> "ImageData":
         """Create ImageData from a numpy array.
 
         Args:
             arr (numpy.ndarray): Numpy array or Numpy masked array.
 
         """
-        if len(arr.shape) < 3:
-            arr = numpy.expand_dims(arr, axis=0)
-
-        if isinstance(arr, numpy.ma.MaskedArray):
-            data = numpy.ma.getdata(arr)
-            mask = ~numpy.logical_or.reduce(numpy.ma.getmaskarray(arr))
-            return cls(data, mask * numpy.uint8(255))
-
+        warnings.warn(
+            "'ImageData.from_array()' has been deprecated and will be removed"
+            "in rio-tiler 6.0.",
+            DeprecationWarning,
+        )
         return cls(arr)
 
     @classmethod
     def from_bytes(cls, data: bytes) -> "ImageData":
         """Create ImageData from bytes.
 
         Args:
@@ -332,21 +395,22 @@
         """
         with MemoryFile(data) as m:
             with m.open() as dataset:
                 indexes = non_alpha_indexes(dataset)
                 if ColorInterp.alpha in dataset.colorinterp:
                     alpha_idx = dataset.colorinterp.index(ColorInterp.alpha) + 1
                     idx = tuple(indexes) + (alpha_idx,)
+                    array = dataset.read(indexes=idx)
 
-                    arr = dataset.read(indexes=idx)
-                    arr, mask = arr[0:-1], arr[-1].astype("uint8")
+                    mask = ~array[-1].astype("bool")
+                    array = numpy.ma.MaskedArray(array[0:-1])
+                    array.mask = mask
 
                 else:
-                    arr = dataset.read(indexes=indexes)
-                    mask = dataset.dataset_mask()
+                    array = dataset.read(indexes=indexes, masked=True)
 
                 stats = []
                 for ix in indexes:
                     tags = dataset.tags(ix)
                     if all(
                         stat in tags
                         for stat in ["STATISTICS_MINIMUM", "STATISTICS_MAXIMUM"]
@@ -354,44 +418,54 @@
                         stat_min = float(tags.get("STATISTICS_MINIMUM"))
                         stat_max = float(tags.get("STATISTICS_MAXIMUM"))
                         stats.append((stat_min, stat_max))
 
                 dataset_statistics = stats if len(stats) == len(indexes) else None
 
                 return cls(
-                    arr,
-                    mask,
+                    array,
                     crs=dataset.crs,
                     bounds=dataset.bounds,
                     dataset_statistics=dataset_statistics,
                 )
 
     @classmethod
     def create_from_list(cls, data: Sequence["ImageData"]) -> "ImageData":
         """Create ImageData from a sequence of ImageData objects.
 
         Args:
             data (sequence): sequence of ImageData.
 
         """
         h, w = zip(*[(img.height, img.width) for img in data])
+
+        # Get cutline mask at highest resolution.
+        max_h, max_w = max(h), max(w)
+        cutline_mask = next(
+            img.cutline_mask
+            for img in data
+            if img.height == max_h and img.width == max_w
+        )
+
         if len(set(h)) > 1 or len(set(w)) > 1:
             warnings.warn(
                 "Cannot concatenate images with different size. Will resize using max width/heigh",
                 UserWarning,
             )
-            max_h, max_w = max(h), max(w)
             for img in data:
                 if img.height == max_h and img.width == max_w:
                     continue
-                img.data = resize_array(img.data, max_h, max_w)
-                img.mask = resize_array(img.mask, max_h, max_w)
+                arr = numpy.ma.MaskedArray(
+                    resize_array(img.array.data, max_h, max_w),
+                    mask=resize_array(img.array.mask * 1, max_h, max_w).astype("bool"),
+                )
+                img.array = arr
+
+        arr = numpy.ma.concatenate([img.array for img in data])
 
-        arr = numpy.concatenate([img.data for img in data])
-        mask = numpy.all([img.mask for img in data], axis=0).astype(numpy.uint8) * 255
         assets = list(
             dict.fromkeys(
                 itertools.chain.from_iterable(
                     [img.assets for img in data if img.assets]
                 )
             )
         )
@@ -411,52 +485,62 @@
         stats = list(
             itertools.chain.from_iterable(
                 [img.dataset_statistics for img in data if img.dataset_statistics]
             )
         )
         dataset_statistics = stats if len(stats) == len(band_names) else None
 
+        metadata = dict(
+            itertools.chain.from_iterable(
+                [img.metadata.items() for img in data if img.metadata]
+            )
+        )
+
         return cls(
             arr,
-            mask,
             assets=assets,
             crs=crs,
             bounds=bounds,
             band_names=band_names,
             dataset_statistics=dataset_statistics,
+            cutline_mask=cutline_mask,
+            metadata=metadata,
         )
 
     def as_masked(self) -> numpy.ma.MaskedArray:
         """return a numpy masked array."""
-        data = numpy.ma.array(self.data)
-        data.mask = self.mask == 0
-        return data
+        warnings.warn(
+            "'ImageData.as_masked' has been deprecated and will be removed"
+            "in rio-tiler 6.0. You can get the masked array directly with `ImageData.array` attribute.",
+            DeprecationWarning,
+        )
+        return self.array
 
     def data_as_image(self) -> numpy.ndarray:
         """Return the data array reshaped into an image processing/visualization software friendly order.
 
         (bands, rows, columns) -> (rows, columns, bands).
 
         """
-        return reshape_as_image(self.data)
+        return reshape_as_image(self.array.data)
 
     @property
     def width(self) -> int:
         """Width of the data array."""
-        return self.data.shape[2]
+        return self.array.shape[2]
 
     @property
     def height(self) -> int:
         """Height of the data array."""
-        return self.data.shape[1]
+        return self.array.shape[1]
 
     @property
     def count(self) -> int:
         """Number of band."""
-        return self.data.shape[0]
+        return self.array.shape[0]
 
     @property
     def transform(self):
         """Returns the affine transform."""
         return (
             from_bounds(*self.bounds, self.width, self.height)
             if self.bounds
@@ -466,43 +550,47 @@
     def rescale(
         self,
         in_range: Sequence[IntervalTuple],
         out_range: Sequence[IntervalTuple] = ((0, 255),),
         out_dtype: Union[str, numpy.number] = "uint8",
     ):
         """Rescale data in place."""
-        self.data = rescale_image(
-            self.data.copy(),
-            self.mask,
+        self.array = rescale_image(
+            self.array.copy(),
             in_range=in_range,
             out_range=out_range,
             out_dtype=out_dtype,
         )
 
     def apply_colormap(self, colormap: ColorMapType) -> "ImageData":
         """Apply colormap to the image data."""
-        data, alpha = apply_cmap(self.data, colormap)
+        data, alpha = apply_cmap(self.array.data, colormap)
+
+        # Use Dataset Mask which is fine
+        # because in theory self.array should be a 1 band image
+        array = numpy.ma.MaskedArray(data)
+        array.mask = numpy.bitwise_and(alpha, self.mask) == 0
+
         return ImageData(
-            data,
-            numpy.bitwise_and(alpha, self.mask),
+            array,
             assets=self.assets,
             crs=self.crs,
             bounds=self.bounds,
             metadata=self.metadata,
         )
 
     def apply_color_formula(self, color_formula: Optional[str]):
         """Apply color-operations formula in place."""
-        out = self.data.copy()
+        out = self.array.data.copy()
         out[out < 0] = 0
 
         for ops in parse_operations(color_formula):
             out = scale_dtype(ops(to_math_type(out)), numpy.uint8)
 
-        self.data = out
+        self.array.data = out
 
     def apply_expression(self, expression: str) -> "ImageData":
         """Apply expression to the image data."""
         blocks = get_expression_blocks(expression)
 
         stats = self.dataset_statistics
         if stats:
@@ -513,57 +601,58 @@
             stats = list(
                 zip(
                     [min(r) for r in zip(*res)],
                     [max(r) for r in zip(*res)],
                 )
             )
 
+        data = apply_expression(blocks, self.band_names, self.array)
+        # NOTE: We use dataset mask when mixing bands
+        data.mask = numpy.logical_or.reduce(self.array.mask)
+
         return ImageData(
-            apply_expression(blocks, self.band_names, self.data),
-            self.mask.copy(),
+            data,
             assets=self.assets,
             crs=self.crs,
             bounds=self.bounds,
             band_names=blocks,
             metadata=self.metadata,
             dataset_statistics=stats,
         )
 
     def resize(
         self,
         height: int,
         width: int,
-        resampling_method: Resampling = "nearest",
+        resampling_method: RIOResampling = "nearest",
     ) -> "ImageData":
         """Resize data and mask."""
-        data = resize_array(self.data, height, width, resampling_method)
-        mask = resize_array(self.mask, height, width, resampling_method)
+        data = resize_array(self.array.data, height, width, resampling_method)
+        mask = resize_array(
+            self.array.mask * 1, height, width, resampling_method
+        ).astype("bool")
 
         return ImageData(
-            data,
-            mask,
+            numpy.ma.MaskedArray(data, mask=mask),
             assets=self.assets,
             crs=self.crs,
             bounds=self.bounds,
             band_names=self.band_names,
             metadata=self.metadata,
             dataset_statistics=self.dataset_statistics,
         )
 
     def clip(self, bbox: BBox) -> "ImageData":
         """Clip data and mask to a bbox."""
         row_slice, col_slice = windows.from_bounds(
             *bbox, transform=self.transform
         ).toslices()
-        data = self.data[:, row_slice, col_slice]
-        mask = self.mask[row_slice, col_slice]
 
         return ImageData(
-            data,
-            mask,
+            self.array[:, row_slice, col_slice].copy(),
             assets=self.assets,
             crs=self.crs,
             bounds=bbox,
             band_names=self.band_names,
             metadata=self.metadata,
             dataset_statistics=self.dataset_statistics,
         )
@@ -588,28 +677,27 @@
 
         Examples:
             >>> img.post_process(in_range=((0, 16000), ))
 
             >>> img.post_process(color_formula="Gamma RGB 4.1")
 
         """
-        data = self.data.copy()
-        mask = self.mask.copy()
+        array = self.array.copy()
 
         if in_range:
-            data = rescale_image(data, mask, in_range, out_dtype=out_dtype, **kwargs)
+            array = rescale_image(array, in_range, out_dtype=out_dtype, **kwargs)
 
         if color_formula:
-            data[data < 0] = 0
+            array[array < 0] = 0
             for ops in parse_operations(color_formula):
-                data = scale_dtype(ops(to_math_type(data)), numpy.uint8)
+                array = scale_dtype(ops(to_math_type(array)), numpy.uint8)
+            array.mask = self.array.mask
 
         return ImageData(
-            data,
-            mask,
+            array,
             crs=self.crs,
             bounds=self.bounds,
             assets=self.assets,
             metadata=self.metadata,
         )
 
     def render(
@@ -635,63 +723,67 @@
 
         if img_format == "GTIFF":
             if "transform" not in kwargs:
                 kwargs.update({"transform": self.transform})
             if "crs" not in kwargs and self.crs:
                 kwargs.update({"crs": self.crs})
 
-        data = self.data.copy()
-        mask = self.mask.copy()
-        datatype_range = self.dataset_statistics or (dtype_ranges[str(data.dtype)],)
+        array = self.array.copy()
+
+        datatype_range = self.dataset_statistics or (dtype_ranges[str(array.dtype)],)
 
         if not colormap:
-            if img_format in ["PNG"] and data.dtype not in ["uint8", "uint16"]:
+            if img_format in ["PNG"] and array.dtype not in ["uint8", "uint16"]:
                 warnings.warn(
-                    f"Invalid type: `{data.dtype}` for the `{img_format}` driver. Data will be rescaled using min/max type bounds or dataset_statistics.",
+                    f"Invalid type: `{array.dtype}` for the `{img_format}` driver. Data will be rescaled using min/max type bounds or dataset_statistics.",
                     InvalidDatatypeWarning,
                 )
-                data = rescale_image(data, mask, in_range=datatype_range)
+                array = rescale_image(array, in_range=datatype_range)
 
-            elif img_format in ["JPEG", "WEBP"] and data.dtype not in ["uint8"]:
+            elif img_format in ["JPEG", "WEBP"] and array.dtype not in ["uint8"]:
                 warnings.warn(
-                    f"Invalid type: `{data.dtype}` for the `{img_format}` driver. Data will be rescaled using min/max type bounds or dataset_statistics.",
+                    f"Invalid type: `{array.dtype}` for the `{img_format}` driver. Data will be rescaled using min/max type bounds or dataset_statistics.",
                     InvalidDatatypeWarning,
                 )
-                data = rescale_image(data, mask, in_range=datatype_range)
+                array = rescale_image(array, in_range=datatype_range)
 
-            elif img_format in ["JP2OPENJPEG"] and data.dtype not in [
+            elif img_format in ["JP2OPENJPEG"] and array.dtype not in [
                 "uint8",
                 "int16",
                 "uint16",
             ]:
                 warnings.warn(
-                    f"Invalid type: `{data.dtype}` for the `{img_format}` driver. Data will be rescaled using min/max type bounds or dataset_statistics.",
+                    f"Invalid type: `{array.dtype}` for the `{img_format}` driver. Data will be rescaled using min/max type bounds or dataset_statistics.",
                     InvalidDatatypeWarning,
                 )
-                data = rescale_image(data, mask, in_range=datatype_range)
+                array = rescale_image(array, in_range=datatype_range)
 
         if add_mask:
             return render(
-                data, mask, img_format=img_format, colormap=colormap, **kwargs
+                array.data,
+                self.mask,  # We use dataset mask for rendering
+                img_format=img_format,
+                colormap=colormap,
+                **kwargs,
             )
 
-        return render(data, img_format=img_format, colormap=colormap, **kwargs)
+        return render(array.data, img_format=img_format, colormap=colormap, **kwargs)
 
     def statistics(
         self,
         categorical: bool = False,
         categories: Optional[List[float]] = None,
         percentiles: Optional[List[int]] = None,
         hist_options: Optional[Dict] = None,
     ) -> Dict[str, BandStatistics]:
         """Return statistics from ImageData."""
         hist_options = hist_options or {}
 
         stats = get_array_statistics(
-            self.as_masked(),
+            self.array,
             categorical=categorical,
             categories=categories,
             percentiles=percentiles,
             **hist_options,
         )
 
         return {
```

### Comparing `rio_tiler-4.1.9/rio_tiler/profiles.py` & `rio_tiler-5.0.0/rio_tiler/profiles.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/reader.py` & `rio_tiler-5.0.0/rio_tiler/reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 """rio-tiler.reader: low level reader."""
 
 import contextlib
 import math
 import warnings
+from enum import IntEnum
 from typing import Callable, Dict, Optional, Tuple, TypedDict, Union
 
 import numpy
 from affine import Affine
 from rasterio import windows
 from rasterio.crs import CRS
-from rasterio.enums import ColorInterp, Resampling
+from rasterio.enums import ColorInterp, MaskFlags, Resampling
 from rasterio.io import DatasetReader, DatasetWriter
 from rasterio.vrt import WarpedVRT
 from rasterio.warp import transform as transform_coords
 from rasterio.warp import transform_bounds
 
 from rio_tiler.constants import WGS84_CRS
 from rio_tiler.errors import InvalidBufferSize, PointOutsideBounds, TileOutsideBounds
 from rio_tiler.models import ImageData, PointData
-from rio_tiler.types import BBox, DataMaskType, Indexes, NoData
+from rio_tiler.types import BBox, Indexes, NoData, RIOResampling, WarpResampling
 from rio_tiler.utils import _requested_tile_aligned_with_internal_tile as is_aligned
 from rio_tiler.utils import get_vrt_transform, has_alpha_band, non_alpha_indexes
 
 
 class Options(TypedDict, total=False):
     """Reader Options."""
 
     force_binary_mask: Optional[bool]
     nodata: Optional[NoData]
     vrt_options: Optional[Dict]
-    resampling_method: Optional[Resampling]
+    resampling_method: Optional[RIOResampling]
+    reproject_method: Optional[WarpResampling]
     unscale: Optional[bool]
-    post_process: Optional[Callable[[numpy.ndarray, numpy.ndarray], DataMaskType]]
+    post_process: Optional[Callable[[numpy.ma.MaskedArray], numpy.ma.MaskedArray]]
 
 
 def _get_width_height(max_size, dataset_height, dataset_width) -> Tuple[int, int]:
     """Get Output Width/Height based on a max_size and dataset shape."""
     if max(dataset_height, dataset_width) < max_size:
         return dataset_height, dataset_width
 
@@ -82,33 +84,35 @@
     width: Optional[int] = None,
     max_size: Optional[int] = None,
     indexes: Optional[Indexes] = None,
     window: Optional[windows.Window] = None,
     force_binary_mask: bool = True,
     nodata: Optional[NoData] = None,
     vrt_options: Optional[Dict] = None,
-    resampling_method: Resampling = "nearest",
+    resampling_method: RIOResampling = "nearest",
+    reproject_method: WarpResampling = "nearest",
     unscale: bool = False,
     post_process: Optional[
-        Callable[[numpy.ndarray, numpy.ndarray], DataMaskType]
+        Callable[[numpy.ma.MaskedArray], numpy.ma.MaskedArray]
     ] = None,
 ) -> ImageData:
     """Low level read function.
 
     Args:
         src_dst (rasterio.io.DatasetReader or rasterio.io.DatasetWriter or rasterio.vrt.WarpedVRT): Rasterio dataset.
         dst_crs (rasterio.crs.CRS, optional): Target coordinate reference system.
         height (int, optional): Output height of the image.
         width (int, optional): Output width of the image.
         max_size (int, optional): Limit output size image if not width and height.
         indexes (sequence of int or int, optional): Band indexes.
         window (rasterio.windows.Window, optional): Window to read.
         nodata (int or float, optional): Overwrite dataset internal nodata value.
         vrt_options (dict, optional): Options to be passed to the rasterio.warp.WarpedVRT class.
-        resampling_method (rasterio.enums.Resampling, optional): Rasterio's resampling algorithm. Defaults to `nearest`.
+        resampling_method (RIOResampling, optional): RasterIO resampling algorithm. Defaults to `nearest`.
+        reproject_method (WarpResampling, optional): WarpKernel resampling algorithm. Defaults to `nearest`.
         force_binary_mask (bool, optional): Cast returned mask to binary values (0 or 255). Defaults to `True`.
         unscale (bool, optional): Apply 'scales' and 'offsets' on output data value. Defaults to `False`.
         post_process (callable, optional): Function to apply on output data and mask values.
 
     Returns:
         ImageData
 
@@ -118,23 +122,25 @@
 
     if max_size and width and height:
         warnings.warn(
             "'max_size' will be ignored with with 'height' and 'width' set.",
             UserWarning,
         )
 
-    resampling = Resampling[resampling_method]
+    io_resampling = Resampling[resampling_method]
+    warp_resampling = Resampling[reproject_method]
+
     dst_crs = dst_crs or src_dst.crs
     with contextlib.ExitStack() as ctx:
         # Use WarpedVRT when Re-projection or Nodata or User VRT Option (cutline)
         if (dst_crs != src_dst.crs) or nodata is not None or vrt_options:
             vrt_params = {
                 "crs": dst_crs,
                 "add_alpha": True,
-                "resampling": resampling,
+                "resampling": warp_resampling,
             }
 
             nodata = nodata if nodata is not None else src_dst.nodata
             if nodata is not None:
                 vrt_params.update(
                     {"nodata": nodata, "add_alpha": False, "src_nodata": nodata}
                 )
@@ -172,78 +178,102 @@
             ):
                 boundless = True
 
         if ColorInterp.alpha in dataset.colorinterp:
             # If dataset has an alpha band we need to get the mask using the alpha band index
             # and then split the data and mask values
             alpha_idx = dataset.colorinterp.index(ColorInterp.alpha) + 1
-            idx = tuple(indexes) + (alpha_idx,)
-            data = dataset.read(
-                indexes=idx,
-                window=window,
-                out_shape=(len(idx), height, width) if height and width else None,
-                resampling=resampling,
-                boundless=boundless,
-            )
-            data, mask = data[0:-1], data[-1].astype("uint8")
+
+            # Read Data and Mask separately
+            # Special case (see https://github.com/rasterio/rasterio/issues/2798)
+            if dataset.dtypes[alpha_idx - 1] != dataset.dtypes[indexes[0] - 1]:
+                values = dataset.read(
+                    indexes=indexes,
+                    window=window,
+                    out_shape=(len(indexes), height, width)
+                    if height and width
+                    else None,
+                    resampling=io_resampling,
+                    boundless=boundless,
+                )
+                mask = dataset.read(
+                    indexes=(alpha_idx,),
+                    window=window,
+                    out_shape=(1, height, width) if height and width else None,
+                    resampling=io_resampling,
+                    boundless=boundless,
+                )
+                data = numpy.ma.MaskedArray(values)
+                data.mask = ~mask.astype("bool")
+
+            else:
+                idx = tuple(indexes) + (alpha_idx,)
+                values = dataset.read(
+                    indexes=idx,
+                    window=window,
+                    out_shape=(len(idx), height, width) if height and width else None,
+                    resampling=io_resampling,
+                    boundless=boundless,
+                )
+                mask = ~values[-1].astype("bool")
+                data = numpy.ma.MaskedArray(values[0:-1])
+                data.mask = mask
 
         else:
             data = dataset.read(
                 indexes=indexes,
                 window=window,
                 out_shape=(len(indexes), height, width) if height and width else None,
-                resampling=resampling,
-                boundless=boundless,
-            )
-            mask = dataset.dataset_mask(
-                window=window,
-                out_shape=(height, width) if height and width else None,
-                resampling=resampling,
+                resampling=io_resampling,
                 boundless=boundless,
+                masked=True,
             )
 
+            # if data has Nodata then we simply make sure the mask == the nodata
+            if dataset.nodata is not None:
+                data.mask |= data == dataset.nodata
+
         stats = []
         for ix in indexes:
             tags = dataset.tags(ix)
             if all(
                 stat in tags for stat in ["STATISTICS_MINIMUM", "STATISTICS_MAXIMUM"]
             ):
                 stat_min = float(tags.get("STATISTICS_MINIMUM"))
                 stat_max = float(tags.get("STATISTICS_MAXIMUM"))
                 stats.append((stat_min, stat_max))
 
         # We only add dataset statistics if we have them for all the indexes
         dataset_statistics = stats if len(stats) == len(indexes) else None
 
+        # TODO: DEPRECATED, masked array are already using bool
         if force_binary_mask:
-            mask = numpy.where(mask != 0, numpy.uint8(255), numpy.uint8(0))
+            pass
 
         if unscale:
             data = data.astype("float32", casting="unsafe")
             numpy.multiply(data, dataset.scales[0], out=data, casting="unsafe")
             numpy.add(data, dataset.offsets[0], out=data, casting="unsafe")
 
         if post_process:
-            data, mask = post_process(data, mask)
+            data = post_process(data)
 
         out_bounds = (
             windows.bounds(window, dataset.transform) if window else dataset.bounds
         )
 
-        img = ImageData(
+        return ImageData(
             data,
-            mask,
             bounds=out_bounds,
             crs=dataset.crs,
             band_names=[f"b{idx}" for idx in indexes],
             dataset_statistics=dataset_statistics,
+            metadata=dataset.tags(),
         )
 
-    return img
-
 
 # flake8: noqa: C901
 def part(
     src_dst: Union[DatasetReader, DatasetWriter, WarpedVRT],
     bounds: BBox,
     height: Optional[int] = None,
     width: Optional[int] = None,
@@ -253,18 +283,19 @@
     indexes: Optional[Indexes] = None,
     minimum_overlap: Optional[float] = None,
     padding: Optional[int] = None,
     buffer: Optional[float] = None,
     force_binary_mask: bool = True,
     nodata: Optional[NoData] = None,
     vrt_options: Optional[Dict] = None,
-    resampling_method: Resampling = "nearest",
+    resampling_method: RIOResampling = "nearest",
+    reproject_method: WarpResampling = "nearest",
     unscale: bool = False,
     post_process: Optional[
-        Callable[[numpy.ndarray, numpy.ndarray], DataMaskType]
+        Callable[[numpy.ma.MaskedArray], numpy.ma.MaskedArray]
     ] = None,
 ) -> ImageData:
     """Read part of a dataset.
 
     Args:
         src_dst (rasterio.io.DatasetReader or rasterio.io.DatasetWriter or rasterio.vrt.WarpedVRT): Rasterio dataset.
         bounds (tuple): Output bounds (left, bottom, right, top). By default the coordinates are considered to be in either the dataset CRS or in the `dst_crs` if set. Use `bounds_crs` to set a specific CRS.
@@ -275,16 +306,16 @@
         bounds_crs (rasterio.crs.CRS, optional): Overwrite bounds Coordinate Reference System.
         indexes (sequence of int or int, optional): Band indexes.
         minimum_overlap (float, optional): Minimum % overlap for which to raise an error with dataset not covering enough of the tile.
         padding (int, optional): Padding to apply to each bbox edge. Helps reduce resampling artefacts along edges. Defaults to `0`.
         buffer (float, optional): Buffer to apply to each bbox edge. Defaults to `0.`.
         nodata (int or float, optional): Overwrite dataset internal nodata value.
         vrt_options (dict, optional): Options to be passed to the rasterio.warp.WarpedVRT class.
-        resampling_method (rasterio.enums.Resampling, optional): Rasterio's resampling algorithm. Defaults to `nearest`.
-        force_binary_mask (bool, optional): Cast returned mask to binary values (0 or 255). Defaults to `True`.
+        resampling_method (RIOResampling, optional): RasterIO resampling algorithm. Defaults to `nearest`.
+        reproject_method (WarpResampling, optional): WarpKernel resampling algorithm. Defaults to `nearest`.
         unscale (bool, optional): Apply 'scales' and 'offsets' on output data value. Defaults to `False`.
         post_process (callable, optional): Function to apply on output data and mask values.
 
     Returns:
         ImageData
 
     """
@@ -369,14 +400,15 @@
             indexes=indexes,
             width=width,
             height=height,
             window=window,
             nodata=nodata,
             vrt_options=vrt_params,
             resampling_method=resampling_method,
+            reproject_method=reproject_method,
             force_binary_mask=force_binary_mask,
             unscale=unscale,
             post_process=post_process,
         )
 
     # else no re-projection needed
     window = windows.from_bounds(*bounds, transform=src_dst.transform)
@@ -400,80 +432,85 @@
         img = read(
             src_dst,
             indexes=indexes,
             width=width,
             height=height,
             window=window,
             resampling_method=resampling_method,
+            reproject_method=reproject_method,
             force_binary_mask=force_binary_mask,
             unscale=unscale,
             post_process=post_process,
         )
+
         return ImageData(
-            data=img.data[:, padding:-padding, padding:-padding],
-            mask=img.mask[padding:-padding, padding:-padding],
+            img.array[:, padding:-padding, padding:-padding],
             bounds=bounds,
             crs=img.crs,
             band_names=img.band_names,
             dataset_statistics=img.dataset_statistics,
+            metadata=img.metadata,
         )
 
     return read(
         src_dst,
         indexes=indexes,
         width=width,
         height=height,
         window=window,
         resampling_method=resampling_method,
+        reproject_method=reproject_method,
         force_binary_mask=force_binary_mask,
         unscale=unscale,
         post_process=post_process,
     )
 
 
 def point(
     src_dst: Union[DatasetReader, DatasetWriter, WarpedVRT],
     coordinates: Tuple[float, float],
     indexes: Optional[Indexes] = None,
     coord_crs: CRS = WGS84_CRS,
     force_binary_mask: bool = True,
     nodata: Optional[NoData] = None,
     vrt_options: Optional[Dict] = None,
-    resampling_method: Resampling = "nearest",
+    resampling_method: RIOResampling = "nearest",
+    reproject_method: WarpResampling = "nearest",
     unscale: bool = False,
     post_process: Optional[
-        Callable[[numpy.ndarray, numpy.ndarray], DataMaskType]
+        Callable[[numpy.ma.MaskedArray], numpy.ma.MaskedArray]
     ] = None,
 ) -> PointData:
     """Read a pixel value for a point.
 
     Args:
         src_dst (rasterio.io.DatasetReader or rasterio.io.DatasetWriter or rasterio.vrt.WarpedVRT): Rasterio dataset.
         coordinates (tuple): Coordinates in form of (X, Y).
         indexes (sequence of int or int, optional): Band indexes.
         coord_crs (rasterio.crs.CRS, optional): Coordinate Reference System of the input coords. Defaults to `epsg:4326`.
         nodata (int or float, optional): Overwrite dataset internal nodata value.
         vrt_options (dict, optional): Options to be passed to the rasterio.warp.WarpedVRT class.
-        resampling_method (rasterio.enums.Resampling, optional): Rasterio's resampling algorithm. Defaults to `nearest`.
+        resampling_method (RIOResampling, optional): RasterIO resampling algorithm. Defaults to `nearest`.
+        reproject_method (WarpResampling, optional): WarpKernel resampling algorithm. Defaults to `nearest`.
         unscale (bool, optional): Apply 'scales' and 'offsets' on output data value. Defaults to `False`.
         post_process (callable, optional): Function to apply on output data and mask values.
 
     Returns:
         PointData
 
     """
     if isinstance(indexes, int):
         indexes = (indexes,)
 
     with contextlib.ExitStack() as ctx:
-        # Use WarpedVRT when Re-projection or Nodata or User VRT Option (cutline)
+        # Use WarpedVRT when User provided Nodata or VRT Option (cutline)
         if nodata is not None or vrt_options:
             vrt_params = {
                 "add_alpha": True,
-                "resampling": Resampling[resampling_method],
+                "resampling": Resampling[reproject_method],
             }
             nodata = nodata if nodata is not None else src_dst.nodata
             if nodata is not None:
                 vrt_params.update(
                     {"nodata": nodata, "add_alpha": False, "src_nodata": nodata}
                 )
 
@@ -507,13 +544,13 @@
             resampling_method=resampling_method,
             force_binary_mask=force_binary_mask,
             unscale=unscale,
             post_process=post_process,
         )
 
     return PointData(
-        img.data[:, 0, 0],
-        numpy.array([img.mask[0, 0]]),
+        img.array[:, 0, 0],
         coordinates=coordinates,
         crs=coord_crs,
         band_names=img.band_names,
+        metadata=dataset.tags(),
     )
```

### Comparing `rio_tiler-4.1.9/rio_tiler/tasks.py` & `rio_tiler-5.0.0/rio_tiler/tasks.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/utils.py` & `rio_tiler-5.0.0/rio_tiler/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,69 +1,40 @@
 """rio_tiler.utils: utility functions."""
 
-import os
 import warnings
 from io import BytesIO
 from typing import Any, Dict, Generator, List, Optional, Sequence, Tuple, Union
 
 import numpy
 import rasterio
 from affine import Affine
-from boto3.session import Session as boto3_session
 from rasterio import windows
 from rasterio.crs import CRS
 from rasterio.dtypes import _gdal_typename
 from rasterio.enums import ColorInterp, MaskFlags, Resampling
+from rasterio.errors import NotGeoreferencedWarning
 from rasterio.features import is_valid_geom
 from rasterio.io import DatasetReader, DatasetWriter, MemoryFile
 from rasterio.rio.helpers import coords
 from rasterio.transform import from_bounds, rowcol
 from rasterio.vrt import WarpedVRT
 from rasterio.warp import calculate_default_transform, transform_geom
 
 from rio_tiler.colormap import apply_cmap
 from rio_tiler.constants import WEB_MERCATOR_CRS
 from rio_tiler.errors import RioTilerError
-from rio_tiler.types import BBox, ColorMapType, IntervalTuple
+from rio_tiler.types import BBox, ColorMapType, IntervalTuple, RIOResampling
 
 
 def _chunks(my_list: Sequence, chuck_size: int) -> Generator[Sequence, None, None]:
     """Yield successive n-sized chunks from l."""
     for i in range(0, len(my_list), chuck_size):
         yield my_list[i : i + chuck_size]
 
 
-def aws_get_object(
-    bucket: str,
-    key: str,
-    request_pays: bool = False,
-    client: boto3_session.client = None,
-) -> bytes:
-    """AWS s3 get object content."""
-    if not client:
-        session = boto3_session()
-        # AWS_S3_ENDPOINT and AWS_HTTPS are GDAL config options of vsis3 driver
-        # https://gdal.org/user/virtual_file_systems.html#vsis3-aws-s3-files
-        endpoint_url = os.environ.get("AWS_S3_ENDPOINT", None)
-        if endpoint_url is not None:
-            use_https = os.environ.get("AWS_HTTPS", "YES")
-            if use_https.upper() in ["YES", "TRUE", "ON"]:
-                endpoint_url = "https://" + endpoint_url
-            else:
-                endpoint_url = "http://" + endpoint_url
-        client = session.client("s3", endpoint_url=endpoint_url)
-
-    params = {"Bucket": bucket, "Key": key}
-    if request_pays or os.environ.get("AWS_REQUEST_PAYER", "").lower() == "requester":
-        params["RequestPayer"] = "requester"
-
-    response = client.get_object(**params)
-    return response["Body"].read()
-
-
 def get_array_statistics(
     data: numpy.ma.MaskedArray,
     categorical: bool = False,
     categories: Optional[List[float]] = None,
     percentiles: Optional[List[int]] = None,
     **kwargs: Any,
 ) -> List[Dict[Any, Any]]:
@@ -139,29 +110,36 @@
                 [out_dict.get(x, 0) for x in h_keys],
                 h_keys,
             ]
         else:
             h_counts, h_keys = numpy.histogram(data[b].compressed(), **kwargs)
             histogram = [h_counts.tolist(), h_keys.tolist()]
 
-        percentiles_values = numpy.percentile(
-            data[b].compressed(), percentiles
-        ).tolist()
+        if valid_pixels:
+            percentiles_values = numpy.percentile(
+                data[b].compressed(), percentiles
+            ).tolist()
+        else:
+            percentiles_values = (numpy.nan,) * len(percentiles_names)
 
         output.append(
             {
                 "min": float(data[b].min()),
                 "max": float(data[b].max()),
                 "mean": float(data[b].mean()),
                 "count": float(data[b].count()),
                 "sum": float(data[b].sum()),
                 "std": float(data[b].std()),
                 "median": float(numpy.ma.median(data[b])),
-                "majority": float(keys[counts.tolist().index(counts.max())].tolist()),
-                "minority": float(keys[counts.tolist().index(counts.min())].tolist()),
+                "majority": float(keys[counts.tolist().index(counts.max())].tolist())
+                if valid_pixels
+                else numpy.nan,
+                "minority": float(keys[counts.tolist().index(counts.min())].tolist())
+                if valid_pixels
+                else numpy.nan,
                 "unique": float(counts.size),
                 **dict(zip(percentiles_names, percentiles_values)),
                 "histogram": histogram,
                 **info_px,
             }
         )
 
@@ -467,15 +445,19 @@
         "count": count + 1 if mask is not None else count,
         "height": height,
         "width": width,
     }
     output_profile.update(creation_options)
 
     with warnings.catch_warnings():
-        warnings.simplefilter("ignore", rasterio.errors.NotGeoreferencedWarning)
+        warnings.filterwarnings(
+            "ignore",
+            category=NotGeoreferencedWarning,
+            module="rasterio",
+        )
         with MemoryFile() as memfile:
             with memfile.open(**output_profile) as dst:
                 dst.write(data, indexes=list(range(1, count + 1)))
 
                 # Use Mask as an alpha band
                 if mask is not None:
                     if ColorInterp.alpha not in dst.colorinterp:
@@ -531,16 +513,14 @@
     src_dst: Union[DatasetReader, DatasetWriter, WarpedVRT],
     poly_coordinates: List,
 ) -> List[str]:
     polygons = []
     for point in poly_coordinates:
         xs, ys = zip(*coords(point))
         src_y, src_x = rowcol(src_dst.transform, xs, ys)
-        src_x = [max(0, min(src_dst.width, x)) for x in src_x]
-        src_y = [max(0, min(src_dst.height, y)) for y in src_y]
         polygon = ", ".join([f"{x} {y}" for x, y in list(zip(src_x, src_y))])
         polygons.append(f"({polygon})")
 
     return polygons
 
 
 def create_cutline(
@@ -557,20 +537,15 @@
         src_dst (rasterio.io.DatasetReader or rasterio.io.DatasetWriter or rasterio.vrt.WarpedVRT): Rasterio dataset.
         geometry (dict): GeoJSON feature or GeoJSON geometry. By default the coordinates are considered to be in the dataset CRS. Use `geometry_crs` to set a specific CRS.
         geometry_crs (rasterio.crs.CRS, optional): Input geometry Coordinate Reference System
     Returns:
         str: WKT geometry in form of `POLYGON ((x y, x y, ...)))
 
     """
-    if "geometry" in geometry:
-        geometry = geometry["geometry"]
-
-    if not is_valid_geom(geometry):
-        raise RioTilerError("Invalid geometry")
-
+    geometry = _validate_shape_input(geometry)
     geom_type = geometry["type"]
 
     if geometry_crs:
         geometry = transform_geom(geometry_crs, src_dst.crs, geometry)
 
     if geom_type == "Polygon":
         polys = ",".join(_convert_to_raster_space(src_dst, geometry["coordinates"]))
@@ -626,26 +601,30 @@
     return f"MEM:::{dataset_options}"
 
 
 def resize_array(
     data: numpy.ndarray,
     height: int,
     width: int,
-    resampling_method: Resampling = "nearest",
+    resampling_method: RIOResampling = "nearest",
 ) -> numpy.ndarray:
     """resize array to a given height and width."""
     out_shape: Union[Tuple[int, int], Tuple[int, int, int]]
     if len(data.shape) == 2:
         out_shape = (height, width)
     else:
         out_shape = (data.shape[0], height, width)
 
     datasetname = _array_gdal_name(data)
     with warnings.catch_warnings():
-        warnings.simplefilter("ignore", rasterio.errors.NotGeoreferencedWarning)
+        warnings.filterwarnings(
+            "ignore",
+            category=NotGeoreferencedWarning,
+            module="rasterio",
+        )
         with rasterio.open(datasetname, "r+") as src:
             # if a 2D array is passed, using indexes=1 makes sure we return an 2D array
             indexes = 1 if len(data.shape) == 2 else None
             return src.read(
                 out_shape=out_shape,
                 indexes=indexes,
                 resampling=Resampling[resampling_method],
@@ -656,7 +635,19 @@
     """Return BBox in correct minx, miny, maxx, maxy order."""
     return (
         min(bounds[0], bounds[2]),
         min(bounds[1], bounds[3]),
         max(bounds[0], bounds[2]),
         max(bounds[1], bounds[3]),
     )
+
+
+def _validate_shape_input(shape: Dict) -> Dict:
+    """Ensure input shape is valid and reduce features to geometry"""
+
+    if "geometry" in shape:
+        shape = shape["geometry"]
+
+    if not is_valid_geom(shape):
+        raise RioTilerError("Invalid geometry")
+
+    return shape
```

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/__init__.py` & `rio_tiler-5.0.0/rio_tiler/cmap_data/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/accent.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/accent.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/accent_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/accent_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/afmhot.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/afmhot.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/afmhot_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/afmhot_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/autumn.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/autumn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/autumn_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/autumn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/binary.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/binary.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/binary_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/binary_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/blues.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/blues.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/blues_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/blues_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/bone.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/bone.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/bone_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/bone_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/brbg.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/brbg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/brbg_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/brbg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/brg.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/brg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/brg_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/brg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/bugn.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/bugn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/bugn_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/bugn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/bupu.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/bupu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/bupu_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/bupu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/bwr.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/bwr.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/bwr_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/bwr_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/cfastie.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/cfastie.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/cividis.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/cividis.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/cividis_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/cividis_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/cmrmap.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/cmrmap.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/cmrmap_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/cmrmap_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/cool.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/cool.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/cool_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/cool_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/coolwarm.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/coolwarm.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/coolwarm_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/coolwarm_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/copper.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/copper.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/copper_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/copper_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/cubehelix.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/cubehelix.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/cubehelix_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/cubehelix_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/dark2.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/dark2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/dark2_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/dark2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/flag.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/flag.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/flag_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/flag_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gist_earth.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gist_earth.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gist_earth_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gist_earth_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gist_gray.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gist_gray.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gist_gray_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gist_gray_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gist_heat.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gist_heat.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gist_heat_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gist_heat_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gist_ncar.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gist_ncar.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gist_ncar_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gist_ncar_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gist_rainbow.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gist_rainbow.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gist_rainbow_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gist_rainbow_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gist_stern.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gist_stern.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gist_stern_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gist_stern_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gist_yarg.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gist_yarg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gist_yarg_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gist_yarg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gnbu.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gnbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gnbu_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gnbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gnuplot.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gnuplot.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gnuplot2.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gnuplot2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gnuplot2_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gnuplot2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gnuplot_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gnuplot_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gray.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gray.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/gray_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/gray_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/greens.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/greens.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/greens_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/greens_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/greys.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/greys.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/greys_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/greys_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/hot.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/hot.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/hot_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/hot_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/hsv.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/hsv.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/hsv_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/hsv_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/inferno.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/inferno.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/inferno_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/inferno_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/jet.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/jet.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/jet_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/jet_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/magma.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/magma.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/magma_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/magma_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/nipy_spectral.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/nipy_spectral.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/nipy_spectral_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/nipy_spectral_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/ocean.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/ocean.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/ocean_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/ocean_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/oranges.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/oranges.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/oranges_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/oranges_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/orrd.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/orrd.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/orrd_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/orrd_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/paired.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/paired.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/paired_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/paired_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/pastel1.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/pastel1.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/pastel1_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/pastel1_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/pastel2.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/pastel2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/pastel2_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/pastel2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/pink.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/pink.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/pink_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/pink_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/piyg.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/piyg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/piyg_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/piyg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/plasma.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/plasma.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/plasma_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/plasma_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/prgn.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/prgn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/prgn_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/prgn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/prism.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/prism.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/prism_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/prism_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/pubu.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/pubu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/pubu_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/pubu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/pubugn.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/pubugn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/pubugn_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/pubugn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/puor.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/puor.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/puor_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/puor_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/purd.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/purd.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/purd_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/purd_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/purples.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/purples.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/purples_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/purples_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/rainbow.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/rainbow.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/rainbow_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/rainbow_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/rdbu.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/rdbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/rdbu_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/rdbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/rdgy.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/rdgy.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/rdgy_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/rdgy_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/rdpu.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/rdpu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/rdpu_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/rdpu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/rdylbu.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/rdylbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/rdylbu_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/rdylbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/rdylgn.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/rdylgn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/rdylgn_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/rdylgn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/reds.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/reds.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/reds_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/reds_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/rplumbo.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/rplumbo.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/schwarzwald.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/schwarzwald.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/seismic.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/seismic.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/seismic_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/seismic_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/set1.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/set1.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/set1_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/set1_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/set2.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/set2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/set2_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/set2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/set3.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/set3.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/set3_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/set3_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/spectral.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/spectral.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/spectral_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/spectral_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/spring.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/spring.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/spring_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/spring_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/summer.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/summer.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/summer_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/summer_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/tab10.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/tab10.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/tab10_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/tab10_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/tab20.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/tab20.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/tab20_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/tab20_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/tab20b.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/tab20b.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/tab20b_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/tab20b_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/tab20c.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/tab20c.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/tab20c_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/tab20c_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/terrain.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/terrain.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/terrain_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/terrain_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/twilight.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/twilight.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/twilight_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/twilight_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/twilight_shifted.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/twilight_shifted.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/twilight_shifted_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/twilight_shifted_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/viridis.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/viridis.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/viridis_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/viridis_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/winter.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/winter.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/winter_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/winter_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/wistia.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/wistia.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/wistia_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/wistia_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/ylgn.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/ylgn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/ylgn_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/ylgn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/ylgnbu.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/ylgnbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/ylgnbu_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/ylgnbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/ylorbr.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/ylorbr.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/ylorbr_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/ylorbr_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/ylorrd.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/ylorrd.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/cmap_data/ylorrd_r.npy` & `rio_tiler-5.0.0/rio_tiler/cmap_data/ylorrd_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/rio_tiler/io/base.py` & `rio_tiler-5.0.0/rio_tiler/io/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -274,14 +274,33 @@
         assets = "|".join(self.assets)
         if asset_as_band:
             _re = re.compile(rf"\b({assets})\b")
         else:
             _re = re.compile(rf"\b({assets})_b\d+\b")
         return tuple(set(re.findall(_re, expression)))
 
+    def _update_statistics(
+        self,
+        img: ImageData,
+        indexes: Optional[Indexes] = None,
+        statistics: Optional[Sequence[Tuple[float, float]]] = None,
+    ):
+        """Update ImageData Statistics from AssetInfo."""
+        if isinstance(indexes, int):
+            indexes = (indexes,)
+
+        if indexes is None:
+            indexes = tuple(range(1, img.count + 1))
+
+        if not img.dataset_statistics and statistics:
+            if max(max(indexes), len(indexes)) > len(statistics):  # type: ignore
+                return
+
+            img.dataset_statistics = [statistics[bidx - 1] for bidx in indexes]
+
     def info(
         self, assets: Union[Sequence[str], str] = None, **kwargs: Any
     ) -> Dict[str, Info]:
         """Return metadata from multiple assets.
 
         Args:
             assets (sequence of str or str, optional): assets to fetch info from. Required keyword argument.
@@ -298,17 +317,17 @@
 
         assets = assets or self.assets
 
         if isinstance(assets, str):
             assets = (assets,)
 
         def _reader(asset: str, **kwargs: Any) -> Dict:
-            asset_meta = self._get_asset_info(asset)
-            url = asset_meta["url"]
-            with self.ctx(**asset_meta.get("env", {})):
+            asset_info = self._get_asset_info(asset)
+            url = asset_info["url"]
+            with self.ctx(**asset_info.get("env", {})):
                 with self.reader(url, tms=self.tms, **self.reader_options) as src:  # type: ignore
                     return src.info()
 
         return multi_values(assets, _reader, **kwargs)
 
     def statistics(
         self,
@@ -340,17 +359,17 @@
         if isinstance(assets, str):
             assets = (assets,)
 
         asset_indexes = asset_indexes or {}
         asset_expression = asset_expression or {}
 
         def _reader(asset: str, *args, **kwargs) -> Dict:
-            asset_meta = self._get_asset_info(asset)
-            url = asset_meta["url"]
-            with self.ctx(**asset_meta.get("env", {})):
+            asset_info = self._get_asset_info(asset)
+            url = asset_info["url"]
+            with self.ctx(**asset_info.get("env", {})):
                 with self.reader(url, tms=self.tms, **self.reader_options) as src:  # type: ignore
                     return src.statistics(
                         *args,
                         indexes=asset_indexes.get(asset, kwargs.pop("indexes", None)),  # type: ignore
                         expression=asset_expression.get(asset),  # type: ignore
                         **kwargs,
                     )
@@ -458,19 +477,31 @@
             )
 
         asset_indexes = asset_indexes or {}
 
         def _reader(asset: str, *args: Any, **kwargs: Any) -> ImageData:
             idx = asset_indexes.get(asset) or kwargs.pop("indexes", None)  # type: ignore
 
-            asset_meta = self._get_asset_info(asset)
-            url = asset_meta["url"]
-            with self.ctx(**asset_meta.get("env", {})):
+            asset_info = self._get_asset_info(asset)
+            url = asset_info["url"]
+            with self.ctx(**asset_info.get("env", {})):
                 with self.reader(url, tms=self.tms, **self.reader_options) as src:  # type: ignore
                     data = src.tile(*args, indexes=idx, **kwargs)
+
+                    self._update_statistics(
+                        data,
+                        indexes=idx,
+                        statistics=asset_info.get("dataset_statistics"),
+                    )
+
+                    metadata = data.metadata or {}
+                    if m := asset_info.get("metadata"):
+                        metadata.update(m)
+                    data.metadata = {asset: metadata}
+
                     if asset_as_band:
                         if len(data.band_names) > 1:
                             raise AssetAsBandError(
                                 "Can't use asset_as_band for multibands asset"
                             )
                         data.band_names = [asset]
                     else:
@@ -524,19 +555,31 @@
             )
 
         asset_indexes = asset_indexes or {}
 
         def _reader(asset: str, *args: Any, **kwargs: Any) -> ImageData:
             idx = asset_indexes.get(asset) or kwargs.pop("indexes", None)  # type: ignore
 
-            asset_meta = self._get_asset_info(asset)
-            url = asset_meta["url"]
-            with self.ctx(**asset_meta.get("env", {})):
+            asset_info = self._get_asset_info(asset)
+            url = asset_info["url"]
+            with self.ctx(**asset_info.get("env", {})):
                 with self.reader(url, tms=self.tms, **self.reader_options) as src:  # type: ignore
                     data = src.part(*args, indexes=idx, **kwargs)
+
+                    self._update_statistics(
+                        data,
+                        indexes=idx,
+                        statistics=asset_info.get("dataset_statistics"),
+                    )
+
+                    metadata = data.metadata or {}
+                    if m := asset_info.get("metadata"):
+                        metadata.update(m)
+                    data.metadata = {asset: metadata}
+
                     if asset_as_band:
                         if len(data.band_names) > 1:
                             raise AssetAsBandError(
                                 "Can't use asset_as_band for multibands asset"
                             )
                         data.band_names = [asset]
                     else:
@@ -588,19 +631,31 @@
             )
 
         asset_indexes = asset_indexes or {}
 
         def _reader(asset: str, **kwargs: Any) -> ImageData:
             idx = asset_indexes.get(asset) or kwargs.pop("indexes", None)  # type: ignore
 
-            asset_meta = self._get_asset_info(asset)
-            url = asset_meta["url"]
-            with self.ctx(**asset_meta.get("env", {})):
+            asset_info = self._get_asset_info(asset)
+            url = asset_info["url"]
+            with self.ctx(**asset_info.get("env", {})):
                 with self.reader(url, tms=self.tms, **self.reader_options) as src:  # type: ignore
                     data = src.preview(indexes=idx, **kwargs)
+
+                    self._update_statistics(
+                        data,
+                        indexes=idx,
+                        statistics=asset_info.get("dataset_statistics"),
+                    )
+
+                    metadata = data.metadata or {}
+                    if m := asset_info.get("metadata"):
+                        metadata.update(m)
+                    data.metadata = {asset: metadata}
+
                     if asset_as_band:
                         if len(data.band_names) > 1:
                             raise AssetAsBandError(
                                 "Can't use asset_as_band for multibands asset"
                             )
                         data.band_names = [asset]
                     else:
@@ -656,19 +711,25 @@
             )
 
         asset_indexes = asset_indexes or {}
 
         def _reader(asset: str, *args, **kwargs: Any) -> PointData:
             idx = asset_indexes.get(asset) or kwargs.pop("indexes", None)  # type: ignore
 
-            asset_meta = self._get_asset_info(asset)
-            url = asset_meta["url"]
-            with self.ctx(**asset_meta.get("env", {})):
+            asset_info = self._get_asset_info(asset)
+            url = asset_info["url"]
+            with self.ctx(**asset_info.get("env", {})):
                 with self.reader(url, tms=self.tms, **self.reader_options) as src:  # type: ignore
                     data = src.point(*args, indexes=idx, **kwargs)
+
+                    metadata = data.metadata or {}
+                    if m := asset_info.get("metadata"):
+                        metadata.update(m)
+                    data.metadata = {asset: metadata}
+
                     if asset_as_band:
                         if len(data.band_names) > 1:
                             raise AssetAsBandError(
                                 "Can't use asset_as_band for multibands asset"
                             )
                         data.band_names = [asset]
                     else:
@@ -722,19 +783,31 @@
             )
 
         asset_indexes = asset_indexes or {}
 
         def _reader(asset: str, *args: Any, **kwargs: Any) -> ImageData:
             idx = asset_indexes.get(asset) or kwargs.pop("indexes", None)  # type: ignore
 
-            asset_meta = self._get_asset_info(asset)
-            url = asset_meta["url"]
-            with self.ctx(**asset_meta.get("env", {})):
+            asset_info = self._get_asset_info(asset)
+            url = asset_info["url"]
+            with self.ctx(**asset_info.get("env", {})):
                 with self.reader(url, tms=self.tms, **self.reader_options) as src:  # type: ignore
                     data = src.feature(*args, indexes=idx, **kwargs)
+
+                    self._update_statistics(
+                        data,
+                        indexes=idx,
+                        statistics=asset_info.get("dataset_statistics"),
+                    )
+
+                    metadata = data.metadata or {}
+                    if m := asset_info.get("metadata"):
+                        metadata.update(m)
+                    data.metadata = {asset: metadata}
+
                     if asset_as_band:
                         if len(data.band_names) > 1:
                             raise AssetAsBandError(
                                 "Can't use asset_as_band for multibands asset"
                             )
                         data.band_names = [asset]
                     else:
@@ -939,14 +1012,16 @@
                 "bands must be passed either via expression or bands options."
             )
 
         def _reader(band: str, *args: Any, **kwargs: Any) -> ImageData:
             url = self._get_band_url(band)
             with self.reader(url, tms=self.tms, **self.reader_options) as src:  # type: ignore
                 data = src.tile(*args, **kwargs)
+                if data.metadata:
+                    data.metadata = {band: data.metadata}
                 data.band_names = [band]  # use `band` as name instead of band index
                 return data
 
         img = multi_arrays(bands, _reader, tile_x, tile_y, tile_z, **kwargs)
 
         if expression:
             return img.apply_expression(expression)
@@ -989,14 +1064,16 @@
                 "bands must be passed either via expression or bands options."
             )
 
         def _reader(band: str, *args: Any, **kwargs: Any) -> ImageData:
             url = self._get_band_url(band)
             with self.reader(url, tms=self.tms, **self.reader_options) as src:  # type: ignore
                 data = src.part(*args, **kwargs)
+                if data.metadata:
+                    data.metadata = {band: data.metadata}
                 data.band_names = [band]  # use `band` as name instead of band index
                 return data
 
         img = multi_arrays(bands, _reader, bbox, **kwargs)
 
         if expression:
             return img.apply_expression(expression)
@@ -1037,14 +1114,16 @@
                 "bands must be passed either via expression or bands options."
             )
 
         def _reader(band: str, **kwargs: Any) -> ImageData:
             url = self._get_band_url(band)
             with self.reader(url, tms=self.tms, **self.reader_options) as src:  # type: ignore
                 data = src.preview(**kwargs)
+                if data.metadata:
+                    data.metadata = {band: data.metadata}
                 data.band_names = [band]  # use `band` as name instead of band index
                 return data
 
         img = multi_arrays(bands, _reader, **kwargs)
 
         if expression:
             return img.apply_expression(expression)
@@ -1089,14 +1168,16 @@
                 "bands must be passed either via expression or bands options."
             )
 
         def _reader(band: str, *args, **kwargs: Any) -> PointData:
             url = self._get_band_url(band)
             with self.reader(url, tms=self.tms, **self.reader_options) as src:  # type: ignore
                 data = src.point(*args, **kwargs)
+                if data.metadata:
+                    data.metadata = {band: data.metadata}
                 data.band_names = [band]  # use `band` as name instead of band index
                 return data
 
         data = multi_points(bands, _reader, lon, lat, **kwargs)
         if expression:
             return data.apply_expression(expression)
 
@@ -1138,14 +1219,16 @@
                 "bands must be passed either via expression or bands options."
             )
 
         def _reader(band: str, *args: Any, **kwargs: Any) -> ImageData:
             url = self._get_band_url(band)
             with self.reader(url, tms=self.tms, **self.reader_options) as src:  # type: ignore
                 data = src.feature(*args, **kwargs)
+                if data.metadata:
+                    data.metadata = {band: data.metadata}
                 data.band_names = [band]  # use `band` as name instead of band index
                 return data
 
         img = multi_arrays(bands, _reader, shape, **kwargs)
 
         if expression:
             return img.apply_expression(expression)
```

### Comparing `rio_tiler-4.1.9/rio_tiler/io/rasterio.py` & `rio_tiler-5.0.0/rio_tiler/io/rasterio.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,38 +8,37 @@
 import numpy
 import rasterio
 from affine import Affine
 from morecantile import BoundingBox, Coords, Tile, TileMatrixSet
 from morecantile.utils import _parse_tile_arg
 from rasterio import transform
 from rasterio.crs import CRS
-from rasterio.enums import Resampling
 from rasterio.features import bounds as featureBounds
-from rasterio.features import geometry_mask
+from rasterio.features import geometry_mask, rasterize
 from rasterio.io import DatasetReader, DatasetWriter, MemoryFile
 from rasterio.rio.overview import get_maximum_overview_level
 from rasterio.transform import from_bounds as transform_from_bounds
 from rasterio.vrt import WarpedVRT
-from rasterio.warp import calculate_default_transform
+from rasterio.warp import calculate_default_transform, transform_geom
 from rasterio.windows import Window
 from rasterio.windows import from_bounds as window_from_bounds
 
 from rio_tiler import reader
 from rio_tiler.constants import WEB_MERCATOR_TMS, WGS84_CRS
 from rio_tiler.errors import (
     ExpressionMixingWarning,
     NoOverviewWarning,
     PointOutsideBounds,
     TileOutsideBounds,
 )
 from rio_tiler.expression import parse_expression
 from rio_tiler.io.base import BaseReader
 from rio_tiler.models import BandStatistics, ImageData, Info, PointData
-from rio_tiler.types import BBox, DataMaskType, Indexes, NumType
-from rio_tiler.utils import create_cutline, has_alpha_band, has_mask_band
+from rio_tiler.types import BBox, Indexes, NumType, RIOResampling
+from rio_tiler.utils import _validate_shape_input, has_alpha_band, has_mask_band
 
 
 @attr.s
 class Reader(BaseReader):
     """Rasterio Reader.
 
     Attributes:
@@ -89,25 +88,38 @@
     @options.default
     def _options_default(self):
         return {}
 
     def __attrs_post_init__(self):
         """Define _kwargs, open dataset and get info."""
         if not self.dataset:
-            dataset = self._ctx_stack.enter_context(rasterio.open(self.input))
-            if dataset.gcps[0]:
-                self.dataset = self._ctx_stack.enter_context(
-                    WarpedVRT(
-                        dataset,
-                        src_crs=dataset.gcps[1],
-                        src_transform=transform.from_gcps(dataset.gcps[0]),
-                    )
+            self.dataset = self._ctx_stack.enter_context(rasterio.open(self.input))
+
+        if self.dataset.gcps[0]:
+            vrt_options = {
+                "src_crs": self.dataset.gcps[1],
+                "src_transform": transform.from_gcps(self.dataset.gcps[0]),
+                "add_alpha": True,
+            }
+
+            if self.dataset.nodata is not None:
+                vrt_options.update(
+                    {
+                        "nodata": self.dataset.nodata,
+                        "add_alpha": False,
+                        "src_nodata": self.dataset.nodata,
+                    }
                 )
-            else:
-                self.dataset = dataset
+
+            if has_alpha_band(self.dataset):
+                vrt_options.update({"add_alpha": False})
+
+            self.dataset = self._ctx_stack.enter_context(
+                WarpedVRT(self.dataset, **vrt_options)
+            )
 
         self.bounds = tuple(self.dataset.bounds)
         self.crs = self.dataset.crs
 
         if self.colormap is None:
             self._get_colormap()
 
@@ -125,18 +137,19 @@
 
     def __exit__(self, exc_type, exc_value, traceback):
         """Support using with Context Managers."""
         self.close()
 
     def _dst_geom_in_tms_crs(self):
         """Return dataset info in TMS projection."""
-        if self.crs != self.tms.rasterio_crs:
+        tms_crs = self.tms.rasterio_crs
+        if self.crs != tms_crs:
             dst_affine, w, h = calculate_default_transform(
                 self.crs,
-                self.tms.rasterio_crs,
+                tms_crs,
                 self.dataset.width,
                 self.dataset.height,
                 *self.dataset.bounds,
             )
         else:
             dst_affine = list(self.dataset.transform)
             w = self.dataset.width
@@ -145,15 +158,15 @@
         return dst_affine, w, h
 
     def get_minzoom(self) -> int:
         """Define dataset minimum zoom level."""
         if self._minzoom is None:
             # We assume the TMS tilesize to be constant over all matrices
             # ref: https://github.com/OSGeo/gdal/blob/dc38aa64d779ecc45e3cd15b1817b83216cf96b8/gdal/frmts/gtiff/cogdriver.cpp#L274
-            tilesize = self.tms.tileMatrix[0].tileWidth
+            tilesize = self.tms.tileMatrices[0].tileWidth
 
             try:
                 dst_affine, w, h = self._dst_geom_in_tms_crs()
 
                 # The minzoom is defined by the resolution of the maximum theoretical overview level
                 # We assume `tilesize`` is the smallest overview size
                 overview_level = get_maximum_overview_level(w, h, minsize=tilesize)
@@ -333,19 +346,20 @@
         """
         if not self.tile_exists(tile_x, tile_y, tile_z):
             raise TileOutsideBounds(
                 f"Tile {tile_z}/{tile_x}/{tile_y} is outside {self.input} bounds"
             )
 
         tile_bounds = self.tms.xy_bounds(Tile(x=tile_x, y=tile_y, z=tile_z))
+        dst_crs = self.tms.rasterio_crs
 
         return self.part(
             tile_bounds,
-            dst_crs=self.tms.rasterio_crs,
-            bounds_crs=None,
+            dst_crs=dst_crs,
+            bounds_crs=dst_crs,
             height=tilesize,
             width=tilesize,
             max_size=None,
             indexes=indexes,
             expression=expression,
             buffer=buffer,
             **kwargs,
@@ -518,38 +532,55 @@
             buffer (int or float, optional): Buffer on each side of the given aoi. It must be a multiple of `0.5`. Output **image size** will be expanded to `output imagesize + 2 * buffer` (e.g 0.5 = 257x257, 1.0 = 258x258).
             kwargs (optional): Options to forward to the `Reader.part` method.
 
         Returns:
             rio_tiler.models.ImageData: ImageData instance with data, mask and input spatial info.
 
         """
+        shape = _validate_shape_input(shape)
+
         if not dst_crs:
             dst_crs = shape_crs
 
         # Get BBOX of the polygon
         bbox = featureBounds(shape)
 
-        cutline = create_cutline(self.dataset, shape, geometry_crs=shape_crs)
         vrt_options = kwargs.pop("vrt_options", {})
-        vrt_options.update({"cutline": cutline})
 
-        return self.part(
+        img = self.part(
             bbox,
             dst_crs=dst_crs,
             bounds_crs=shape_crs,
             indexes=indexes,
             expression=expression,
             max_size=max_size,
             width=width,
             height=height,
             vrt_options=vrt_options,
             buffer=buffer,
             **kwargs,
         )
 
+        if dst_crs != shape_crs:
+            shape = transform_geom(shape_crs, dst_crs, shape)
+
+        cutline_mask = rasterize(
+            [shape],
+            out_shape=(img.height, img.width),
+            transform=img.transform,
+            all_touched=True,  # Necesary for matching masks at different resolutions
+            default_value=0,
+            fill=1,
+            dtype="uint8",
+        ).astype("bool")
+        img.cutline_mask = cutline_mask
+        img.array.mask = numpy.where(~cutline_mask, img.array.mask, True)
+
+        return img
+
     def read(
         self,
         indexes: Optional[Indexes] = None,
         expression: Optional[str] = None,
         **kwargs: Any,
     ) -> ImageData:
         """Read the Dataset.
@@ -663,31 +694,31 @@
         tile_x: int,
         tile_y: int,
         tile_z: int,
         tilesize: int = 256,
         indexes: Optional[Indexes] = None,
         expression: Optional[str] = None,
         force_binary_mask: bool = True,
-        resampling_method: Resampling = "nearest",
+        resampling_method: RIOResampling = "nearest",
         unscale: bool = False,
         post_process: Optional[
-            Callable[[numpy.ndarray, numpy.ndarray], DataMaskType]
+            Callable[[numpy.ma.MaskedArray], numpy.ma.MaskedArray]
         ] = None,
     ) -> ImageData:
         """Read a Web Map tile from an Image.
 
         Args:
             tile_x (int): Tile's horizontal index.
             tile_y (int): Tile's vertical index.
             tile_z (int): Tile's zoom level index.
             tilesize (int, optional): Output image size. Defaults to `256`.
             indexes (int or sequence of int, optional): Band indexes.
             expression (str, optional): rio-tiler expression (e.g. b1/b2+b3).
             force_binary_mask (bool, optional): Cast returned mask to binary values (0 or 255). Defaults to `True`.
-            resampling_method (rasterio.enums.Resampling, optional): Rasterio's resampling algorithm. Defaults to `nearest`.
+            resampling_method (RIOResampling, optional): RasterIO resampling algorithm. Defaults to `nearest`.
             unscale (bool, optional): Apply 'scales' and 'offsets' on output data value. Defaults to `False`.
             post_process (callable, optional): Function to apply on output data and mask values.
 
         Returns:
             rio_tiler.models.ImageData: ImageData instance with data, mask and tile spatial info.
 
         """
@@ -716,31 +747,31 @@
         bbox: BBox,
         indexes: Optional[Union[int, Sequence]] = None,
         expression: Optional[str] = None,
         max_size: Optional[int] = None,
         height: Optional[int] = None,
         width: Optional[int] = None,
         force_binary_mask: bool = True,
-        resampling_method: Resampling = "nearest",
+        resampling_method: RIOResampling = "nearest",
         unscale: bool = False,
         post_process: Optional[
-            Callable[[numpy.ndarray, numpy.ndarray], DataMaskType]
+            Callable[[numpy.ma.MaskedArray], numpy.ma.MaskedArray]
         ] = None,
     ) -> ImageData:
         """Read part of an Image.
 
         Args:
             bbox (tuple): Output bounds (left, bottom, right, top).
             indexes (sequence of int or int, optional): Band indexes.
             expression (str, optional): rio-tiler expression (e.g. b1/b2+b3).
             max_size (int, optional): Limit the size of the longest dimension of the dataset read, respecting bounds X/Y aspect ratio.
             height (int, optional): Output height of the array.
             width (int, optional): Output width of the array.
             force_binary_mask (bool, optional): Cast returned mask to binary values (0 or 255). Defaults to `True`.
-            resampling_method (rasterio.enums.Resampling, optional): Rasterio's resampling algorithm. Defaults to `nearest`.
+            resampling_method (RIOResampling, optional): RasterIO resampling algorithm. Defaults to `nearest`.
             unscale (bool, optional): Apply 'scales' and 'offsets' on output data value. Defaults to `False`.
             post_process (callable, optional): Function to apply on output data and mask values.
 
         Returns:
             rio_tiler.models.ImageData: ImageData instance with data, mask and input spatial info.
 
         """
@@ -777,15 +808,15 @@
         self,
         x: float,
         y: float,
         indexes: Optional[Indexes] = None,
         expression: Optional[str] = None,
         unscale: bool = False,
         post_process: Optional[
-            Callable[[numpy.ndarray, numpy.ndarray], DataMaskType]
+            Callable[[numpy.ma.MaskedArray], numpy.ma.MaskedArray]
         ] = None,
     ) -> PointData:
         """Read a pixel value from an Image.
 
         Args:
             lon (float): X coordinate.
             lat (float): Y coordinate.
@@ -806,16 +837,15 @@
             expression=expression,
             unscale=unscale,
             post_process=post_process,
             window=Window(col_off=x, row_off=y, width=1, height=1),
         )
 
         return PointData(
-            img.data[:, 0, 0],
-            numpy.array([img.mask[0, 0]]),
+            img.array[:, 0, 0],
             assets=img.assets,
             coordinates=self.dataset.xy(x, y),
             crs=self.dataset.crs,
             band_names=img.band_names,
         )
 
     def feature(  # type: ignore
@@ -823,18 +853,18 @@
         shape: Dict,
         indexes: Optional[Indexes] = None,
         expression: Optional[str] = None,
         max_size: Optional[int] = None,
         height: Optional[int] = None,
         width: Optional[int] = None,
         force_binary_mask: bool = True,
-        resampling_method: Resampling = "nearest",
+        resampling_method: RIOResampling = "nearest",
         unscale: bool = False,
         post_process: Optional[
-            Callable[[numpy.ndarray, numpy.ndarray], DataMaskType]
+            Callable[[numpy.ma.MaskedArray], numpy.ma.MaskedArray]
         ] = None,
     ) -> ImageData:
         """Read part of an Image defined by a geojson feature."""
         bbox = featureBounds(shape)
 
         # If Image Origin is top Left (non-geo) we need to invert the bbox
         bbox = [bbox[0], bbox[3], bbox[2], bbox[1]]
@@ -848,10 +878,10 @@
             force_binary_mask=force_binary_mask,
             resampling_method=resampling_method,
             unscale=unscale,
             post_process=post_process,
         )
 
         shape = shape.get("geometry", shape)
-        mask = geometry_mask([shape], (img.height, img.width), self.transform)
-        img.mask = mask * 255
+        img.array.mask = geometry_mask([shape], (img.height, img.width), self.transform)
+
         return img
```

### Comparing `rio_tiler-4.1.9/rio_tiler/io/xarray.py` & `rio_tiler-5.0.0/rio_tiler/io/xarray.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 import warnings
 from typing import Any, Dict, List, Optional
 
 import attr
 from morecantile import Tile, TileMatrixSet
 from rasterio.crs import CRS
 from rasterio.enums import Resampling
-from rasterio.features import is_valid_geom
 from rasterio.rio.overview import get_maximum_overview_level
 from rasterio.transform import from_bounds, rowcol
 from rasterio.warp import calculate_default_transform
 from rasterio.warp import transform as transform_coords
 
 from rio_tiler.constants import WEB_MERCATOR_TMS, WGS84_CRS
-from rio_tiler.errors import PointOutsideBounds, RioTilerError, TileOutsideBounds
+from rio_tiler.errors import PointOutsideBounds, TileOutsideBounds
 from rio_tiler.io.base import BaseReader
 from rio_tiler.models import BandStatistics, ImageData, Info, PointData
-from rio_tiler.types import BBox
+from rio_tiler.types import BBox, NoData, WarpResampling
+from rio_tiler.utils import _validate_shape_input
 
 try:
     import xarray
 except ImportError:  # pragma: nocover
     xarray = None  # type: ignore
 
 try:
@@ -76,18 +76,19 @@
             d
             for d in self.input.dims
             if d not in [self.input.rio.x_dim, self.input.rio.y_dim]
         ]
 
     def _dst_geom_in_tms_crs(self):
         """Return dataset info in TMS projection."""
-        if self.crs != self.tms.rasterio_crs:
+        tms_crs = self.tms.rasterio_crs
+        if self.crs != tms_crs:
             dst_affine, w, h = calculate_default_transform(
                 self.crs,
-                self.tms.rasterio_crs,
+                tms_crs,
                 self.input.rio.width,
                 self.input.rio.height,
                 *self.bounds,
             )
         else:
             dst_affine = list(self.input.rio.transform())
             w = self.input.rio.width
@@ -96,15 +97,15 @@
         return dst_affine, w, h
 
     def get_minzoom(self) -> int:
         """Define dataset minimum zoom level."""
         if self._minzoom is None:
             # We assume the TMS tilesize to be constant over all matrices
             # ref: https://github.com/OSGeo/gdal/blob/dc38aa64d779ecc45e3cd15b1817b83216cf96b8/gdal/frmts/gtiff/cogdriver.cpp#L274
-            tilesize = self.tms.tileMatrix[0].tileWidth
+            tilesize = self.tms.tileMatrices[0].tileWidth
 
             try:
                 dst_affine, w, h = self._dst_geom_in_tms_crs()
 
                 # The minzoom is defined by the resolution of the maximum theoretical overview level
                 # We assume `tilesize`` is the smallest overview size
                 overview_level = get_maximum_overview_level(w, h, minsize=tilesize)
@@ -153,14 +154,19 @@
         return self.get_minzoom()
 
     @property
     def maxzoom(self):
         """Return dataset maxzoom."""
         return self.get_maxzoom()
 
+    @property
+    def band_names(self) -> List[str]:
+        """Return list of `band names` in DataArray."""
+        return [str(band) for d in self._dims for band in self.input[d].values]
+
     def info(self) -> Info:
         """Return xarray.DataArray info."""
         bands = [str(band) for d in self._dims for band in self.input[d].values]
         metadata = [band.attrs for d in self._dims for band in self.input[d]]
 
         meta = {
             "bounds": self.geographic_bounds,
@@ -192,112 +198,140 @@
 
     def tile(
         self,
         tile_x: int,
         tile_y: int,
         tile_z: int,
         tilesize: int = 256,
-        resampling_method: Resampling = "nearest",
+        resampling_method: WarpResampling = "nearest",
+        auto_expand: bool = True,
+        nodata: Optional[NoData] = None,
     ) -> ImageData:
         """Read a Web Map tile from a dataset.
 
         Args:
             tile_x (int): Tile's horizontal index.
             tile_y (int): Tile's vertical index.
             tile_z (int): Tile's zoom level index.
             tilesize (int, optional): Output image size. Defaults to `256`.
-            resampling_method (rasterio.enums.Resampling, optional): Rasterio's resampling algorithm. Defaults to `nearest`.
+            resampling_method (WarpResampling, optional): WarpKernel resampling algorithm. Defaults to `nearest`.
+            auto_expand (boolean, optional): When True, rioxarray's clip_box will expand clip search if only 1D raster found with clip. When False, will throw `OneDimensionalRaster` error if only 1 x or y data point is found. Defaults to True.
 
         Returns:
             rio_tiler.models.ImageData: ImageData instance with data, mask and tile spatial info.
 
         """
         if not self.tile_exists(tile_x, tile_y, tile_z):
             raise TileOutsideBounds(
                 f"Tile {tile_z}/{tile_x}/{tile_y} is outside bounds"
             )
 
+        ds = self.input
+        if nodata is not None:
+            ds = ds.rio.write_nodata(nodata)
+
         tile_bounds = self.tms.xy_bounds(Tile(x=tile_x, y=tile_y, z=tile_z))
+        dst_crs = self.tms.rasterio_crs
 
         # Create source array by clipping the xarray dataset to extent of the tile.
-        ds = self.input.rio.clip_box(*tile_bounds, crs=self.tms.rasterio_crs)
+        ds = ds.rio.clip_box(
+            *tile_bounds,
+            crs=dst_crs,
+            auto_expand=auto_expand,
+        )
         ds = ds.rio.reproject(
-            self.tms.rasterio_crs,
+            dst_crs,
             shape=(tilesize, tilesize),
             transform=from_bounds(*tile_bounds, height=tilesize, width=tilesize),
             resampling=Resampling[resampling_method],
+            nodata=nodata,
         )
 
         # Forward valid_min/valid_max to the ImageData object
         minv, maxv = ds.attrs.get("valid_min"), ds.attrs.get("valid_max")
         stats = None
-        if minv is not None and maxv is not None:
+        if minv is not None and maxv is not None and nodata not in [minv, maxv]:
             stats = ((minv, maxv),) * ds.rio.count
 
-        band_names = [str(band) for d in self._dims for band in self.input[d].values]
+        arr = ds.to_masked_array()
+        arr.mask |= arr.data == ds.rio.nodata
 
         return ImageData(
-            ds.data,
+            arr,
             bounds=tile_bounds,
-            crs=self.tms.rasterio_crs,
+            crs=dst_crs,
             dataset_statistics=stats,
-            band_names=band_names,
+            band_names=self.band_names,
         )
 
     def part(
         self,
         bbox: BBox,
         dst_crs: Optional[CRS] = None,
         bounds_crs: CRS = WGS84_CRS,
-        resampling_method: Resampling = "nearest",
+        resampling_method: WarpResampling = "nearest",
+        auto_expand: bool = True,
+        nodata: Optional[NoData] = None,
     ) -> ImageData:
         """Read part of a dataset.
 
         Args:
             bbox (tuple): Output bounds (left, bottom, right, top) in target crs ("dst_crs").
             dst_crs (rasterio.crs.CRS, optional): Overwrite target coordinate reference system.
             bounds_crs (rasterio.crs.CRS, optional): Bounds Coordinate Reference System. Defaults to `epsg:4326`.
-            resampling_method (rasterio.enums.Resampling, optional): Rasterio's resampling algorithm. Defaults to `nearest`.
+            resampling_method (WarpResampling, optional): WarpKernel resampling algorithm. Defaults to `nearest`.
+            auto_expand (boolean, optional): When True, rioxarray's clip_box will expand clip search if only 1D raster found with clip. When False, will throw `OneDimensionalRaster` error if only 1 x or y data point is found. Defaults to True.
 
         Returns:
             rio_tiler.models.ImageData: ImageData instance with data, mask and input spatial info.
 
         """
         dst_crs = dst_crs or bounds_crs
-        ds = self.input.rio.clip_box(*bbox, crs=bounds_crs)
+
+        ds = self.input
+        if nodata is not None:
+            ds = ds.rio.write_nodata(nodata)
+
+        ds = ds.rio.clip_box(
+            *bbox,
+            crs=bounds_crs,
+            auto_expand=auto_expand,
+        )
 
         if dst_crs != self.crs:
             dst_transform, w, h = calculate_default_transform(
                 self.crs,
                 dst_crs,
                 ds.rio.width,
                 ds.rio.height,
                 *ds.rio.bounds(),
             )
             ds = ds.rio.reproject(
                 dst_crs,
                 shape=(h, w),
                 transform=dst_transform,
                 resampling=Resampling[resampling_method],
+                nodata=nodata,
             )
 
         # Forward valid_min/valid_max to the ImageData object
         minv, maxv = ds.attrs.get("valid_min"), ds.attrs.get("valid_max")
         stats = None
         if minv is not None and maxv is not None:
             stats = ((minv, maxv),) * ds.rio.count
 
-        band_names = [str(band) for d in self._dims for band in self.input[d].values]
+        arr = ds.to_masked_array()
+        arr.mask |= arr.data == ds.rio.nodata
 
         return ImageData(
-            ds.data,
+            arr,
             bounds=ds.rio.bounds(),
             crs=ds.rio.crs,
             dataset_statistics=stats,
-            band_names=band_names,
+            band_names=self.band_names,
         )
 
     def preview(
         self,
         max_size: int = 1024,
         height: Optional[int] = None,
         width: Optional[int] = None,
@@ -316,14 +350,15 @@
         raise NotImplementedError
 
     def point(
         self,
         lon: float,
         lat: float,
         coord_crs: CRS = WGS84_CRS,
+        nodata: Optional[NoData] = None,
     ) -> PointData:
         """Read a pixel value from a dataset.
 
         Args:
             lon (float): Longitude.
             lat (float): Latitude.
             coord_crs (rasterio.crs.CRS, optional): Coordinate Reference System of the input coords. Defaults to `epsg:4326`.
@@ -336,77 +371,86 @@
 
         if not (
             (self.bounds[0] < ds_lon[0] < self.bounds[2])
             and (self.bounds[1] < ds_lat[0] < self.bounds[3])
         ):
             raise PointOutsideBounds("Point is outside dataset bounds")
 
-        y, x = rowcol(self.input.rio.transform(), ds_lon, ds_lat)
+        ds = self.input
+        if nodata is not None:
+            ds = ds.rio.write_nodata(nodata)
+
+        y, x = rowcol(ds.rio.transform(), ds_lon, ds_lat)
 
-        band_names = [str(band) for d in self._dims for band in self.input[d].values]
+        arr = ds[:, y[0], x[0]].to_masked_array()
+        arr.mask |= arr.data == ds.rio.nodata
 
         return PointData(
-            self.input.data[:, y[0], x[0]],
+            arr,
             coordinates=(lon, lat),
             crs=coord_crs,
-            band_names=band_names,
+            band_names=self.band_names,
         )
 
     def feature(
         self,
         shape: Dict,
         dst_crs: Optional[CRS] = None,
         shape_crs: CRS = WGS84_CRS,
-        resampling_method: Resampling = "nearest",
+        resampling_method: WarpResampling = "nearest",
+        nodata: Optional[NoData] = None,
     ) -> ImageData:
         """Read part of a dataset defined by a geojson feature.
 
         Args:
             shape (dict): Valid GeoJSON feature.
             dst_crs (rasterio.crs.CRS, optional): Overwrite target coordinate reference system.
             shape_crs (rasterio.crs.CRS, optional): Input geojson coordinate reference system. Defaults to `epsg:4326`.
+            resampling_method (WarpResampling, optional): WarpKernel resampling algorithm. Defaults to `nearest`.
 
         Returns:
             rio_tiler.models.ImageData: ImageData instance with data, mask and input spatial info.
 
         """
         if not dst_crs:
             dst_crs = shape_crs
 
-        if "geometry" in shape:
-            shape = shape["geometry"]
+        shape = _validate_shape_input(shape)
 
-        if not is_valid_geom(shape):
-            raise RioTilerError("Invalid geometry")
+        ds = self.input
+        if nodata is not None:
+            ds = ds.rio.write_nodata(nodata)
 
-        ds = self.input.rio.clip([shape], crs=shape_crs)
+        ds = ds.rio.clip([shape], crs=shape_crs)
 
         if dst_crs != self.crs:
             dst_transform, w, h = calculate_default_transform(
                 self.crs,
                 dst_crs,
                 ds.rio.width,
                 ds.rio.height,
                 *ds.rio.bounds(),
             )
             ds = ds.rio.reproject(
                 dst_crs,
                 shape=(h, w),
                 transform=dst_transform,
                 resampling=Resampling[resampling_method],
+                nodata=nodata,
             )
 
         # Forward valid_min/valid_max to the ImageData object
         minv, maxv = ds.attrs.get("valid_min"), ds.attrs.get("valid_max")
         stats = None
         if minv is not None and maxv is not None:
             stats = ((minv, maxv),) * ds.rio.count
 
-        band_names = [str(band) for d in self._dims for band in self.input[d].values]
+        arr = ds.to_masked_array()
+        arr.mask |= arr.data == ds.rio.nodata
 
         return ImageData(
-            ds.data,
+            arr,
             bounds=ds.rio.bounds(),
             crs=ds.rio.crs,
             dataset_statistics=stats,
-            band_names=band_names,
+            band_names=self.band_names,
         )
```

### Comparing `rio_tiler-4.1.9/rio_tiler/mosaic/reader.py` & `rio_tiler-5.0.0/rio_tiler/mosaic/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """rio_tiler.mosaic: create tile from multiple assets."""
 
 from inspect import isclass
 from typing import Any, Callable, List, Optional, Sequence, Tuple, Type, Union, cast
 
-import numpy
 from rasterio.crs import CRS
 
 from rio_tiler.constants import MAX_THREADS
 from rio_tiler.errors import (
     EmptyMosaicError,
     InvalidMosaicMethod,
     PointOutsideBounds,
@@ -85,46 +84,41 @@
 
     for chunks in _chunks(mosaic_assets, chunk_size):
         tasks = create_tasks(reader, chunks, threads, *args, **kwargs)
         for img, asset in filter_tasks(
             tasks,
             allowed_exceptions=allowed_exceptions,
         ):
-            if isinstance(img, tuple):
-                img = ImageData(*img)
-
             crs = img.crs
             bounds = img.bounds
             band_names = img.band_names
 
+            pixel_selection.cutline_mask = img.cutline_mask
+
             assets_used.append(asset)
-            pixel_selection.feed(img.as_masked())
+            pixel_selection.feed(img.array)
 
-            if pixel_selection.is_done:
-                data, mask = pixel_selection.data
+            if pixel_selection.is_done and pixel_selection.data is not None:
                 return (
                     ImageData(
-                        data,
-                        mask,
+                        pixel_selection.data,
                         assets=assets_used,
                         crs=crs,
                         bounds=bounds,
                         band_names=band_names,
                     ),
                     assets_used,
                 )
 
-    data, mask = pixel_selection.data
-    if data is None:
+    if pixel_selection.data is None:
         raise EmptyMosaicError("Method returned an empty array")
 
     return (
         ImageData(
-            data,
-            mask,
+            pixel_selection.data,
             assets=assets_used,
             crs=crs,
             bounds=bounds,
             band_names=band_names,
         ),
         assets_used,
     )
@@ -146,19 +140,19 @@
 
         mosaic_assets (sequence): List of assets.
         reader (callable): Reader function. The function MUST take `(asset, *args, **kwargs)` as arguments, and MUST return a PointData object.
         args (Any): Argument to forward to the reader function.
         pixel_selection (MosaicMethod, optional): Instance of MosaicMethodBase class. Defaults to `rio_tiler.mosaic.methods.defaults.FirstMethod`.
         chunk_size (int, optional): Control the number of asset to process per loop.
         threads (int, optional): Number of threads to use. If <= 1, runs single threaded without an event loop. By default reads from the MAX_THREADS environment variable, and if not found defaults to multiprocessing.cpu_count() * 5.
-        allowed_exceptions (tuple, optional): List of exceptions which will be ignored. Note: `TileOutsideBounds` is likely to be raised and should be included in the allowed_exceptions. Defaults to `(TileOutsideBounds, )`.
+        allowed_exceptions (tuple, optional): List of exceptions which will be ignored. Note: `PointOutsideBounds` is likely to be raised and should be included in the allowed_exceptions. Defaults to `(TileOutsideBounds, )`.
         kwargs (optional): Reader callable's keywords options.
 
     Returns:
-        tuple: ImageData and assets (list).
+        tuple: PointData and assets (list).
 
     Examples:
         >>> def reader(asset: str, *args, **kwargs) -> PointData:
                 with Reader(asset) as src:
                     return src.point(*args, **kwargs)
 
             pt = mosaic_point_reader(["cog.tif", "cog2.tif"], reader, 0, 0)
@@ -191,38 +185,34 @@
             allowed_exceptions=allowed_exceptions,
         ):
             crs = pt.crs
             coordinates = pt.coordinates
             band_names = pt.band_names
 
             assets_used.append(asset)
-            pixel_selection.feed(pt.as_masked())
+            pixel_selection.feed(pt.array)
 
-            if pixel_selection.is_done:
-                data, mask = pixel_selection.data
+            if pixel_selection.is_done and pixel_selection.data is not None:
                 return (
                     PointData(
-                        data,
-                        numpy.array([mask], dtype="uint8"),
+                        pixel_selection.data,
                         assets=assets_used,
                         crs=crs,
                         coordinates=coordinates,
                         band_names=band_names,
                     ),
                     assets_used,
                 )
 
-    data, mask = pixel_selection.data
-    if data is None:
+    if pixel_selection.data is None:
         raise EmptyMosaicError("Method returned an empty array")
 
     return (
         PointData(
-            data,
-            numpy.array([mask], dtype="uint8"),
+            pixel_selection.data,
             assets=assets_used,
             crs=crs,
             coordinates=coordinates,
             band_names=band_names,
         ),
         assets_used,
     )
```

### Comparing `rio_tiler-4.1.9/rio_tiler/mosaic/methods/base.py` & `rio_tiler-5.0.0/rio_tiler/mosaic/methods/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 """rio-tiler.mosaic.methods abc class."""
 
 import abc
-from typing import Optional, Tuple
+from dataclasses import dataclass, field
+from typing import Optional
 
 import numpy
 
 
+@dataclass
 class MosaicMethodBase(abc.ABC):
     """Abstract base class for rio-tiler-mosaic methods objects."""
 
-    def __init__(self):
-        """Init backend."""
-        self.tile: Optional[numpy.ma.MaskedArray] = None
-        self.exit_when_filled: bool = False
+    mosaic: Optional[numpy.ma.MaskedArray] = field(default=None, init=False)
+    exit_when_filled: bool = field(default=False, init=False)
+    cutline_mask: Optional[numpy.ndarray] = field(default=None, init=False)
 
     @property
     def is_done(self) -> bool:
-        """Check if the tile filling is done.
+        """Check if the mosaic filling is done.
 
         Returns:
             bool
 
         """
-        if self.tile is None:
+        if self.mosaic is None:
             return False
 
-        if self.exit_when_filled and not numpy.ma.is_masked(self.tile):
-            return True
+        if self.exit_when_filled:
+            if (
+                self.cutline_mask is not None
+                and numpy.sum(numpy.where(~self.cutline_mask, self.mosaic.mask, False))
+                == 0
+            ):
+                return True
+            elif not numpy.ma.is_masked(self.mosaic):
+                return True
 
         return False
 
     @property
-    def data(self) -> Tuple[Optional[numpy.ndarray], Optional[numpy.ndarray]]:
-        """Return data and mask."""
-        if self.tile is not None:
-            data = numpy.ma.getdata(self.tile)
-            mask = ~numpy.logical_or.reduce(numpy.ma.getmaskarray(self.tile))
-            return (data, mask * numpy.uint8(255))
-
-        else:
-            return None, None
+    def data(self) -> Optional[numpy.ma.MaskedArray]:
+        """Return data."""
+        return self.mosaic
 
     @abc.abstractmethod
-    def feed(self, tile: numpy.ma.MaskedArray):
-        """Fill mosaic tile.
+    def feed(self, array: numpy.ma.MaskedArray):
+        """Fill mosaic array.
 
         Args:
-            tile (numpy.ma.ndarray): data
+            array (numpy.ma.ndarray): data
 
         """
```

### Comparing `rio_tiler-4.1.9/rio_tiler/mosaic/methods/defaults.py` & `rio_tiler-5.0.0/rio_tiler/mosaic/methods/defaults.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,205 +1,190 @@
 """rio_tiler.mosaic.methods.defaults: default mosaic filling methods."""
 
-from typing import List, Optional, Tuple
+from dataclasses import dataclass, field
+from typing import List, Optional
 
 import numpy
 
 from rio_tiler.mosaic.methods.base import MosaicMethodBase
 
 
+@dataclass
 class FirstMethod(MosaicMethodBase):
-    """Feed the mosaic tile with the first pixel available."""
+    """Feed the mosaic array with the first pixel available."""
 
-    def __init__(self):
-        """Overwrite base and init First method."""
-        super(FirstMethod, self).__init__()
-        self.exit_when_filled = True
-
-    def feed(self, tile: Optional[numpy.ma.MaskedArray]):
-        """Add data to tile."""
-        if self.tile is None:
-            self.tile = tile
-
-        pidex = self.tile.mask & ~tile.mask
-
-        mask = numpy.where(pidex, tile.mask, self.tile.mask)
-        self.tile = numpy.ma.where(pidex, tile, self.tile)
-        self.tile.mask = mask
+    exit_when_filled: bool = field(default=True, init=False)
 
+    def feed(self, array: Optional[numpy.ma.MaskedArray]):
+        """Add data to the mosaic array."""
+        if self.mosaic is None:
+            self.mosaic = array
 
+        else:
+            pidex = self.mosaic.mask & ~array.mask
+
+            mask = numpy.where(pidex, array.mask, self.mosaic.mask)
+            self.mosaic = numpy.ma.where(pidex, array, self.mosaic)
+            self.mosaic.mask = mask
+
+
+@dataclass
 class HighestMethod(MosaicMethodBase):
-    """Feed the mosaic tile with the highest pixel values."""
+    """Feed the mosaic array with the highest pixel values."""
 
-    def feed(self, tile: Optional[numpy.ma.MaskedArray]):
-        """Add data to tile."""
-        if self.tile is None:
-            self.tile = tile
-
-        pidex = (
-            numpy.bitwise_and(tile.data > self.tile.data, ~tile.mask) | self.tile.mask
-        )
-
-        mask = numpy.where(pidex, tile.mask, self.tile.mask)
-        self.tile = numpy.ma.where(pidex, tile, self.tile)
-        self.tile.mask = mask
+    def feed(self, array: Optional[numpy.ma.MaskedArray]):
+        """Add data to the mosaic array."""
+        if self.mosaic is None:
+            self.mosaic = array
 
+        else:
+            pidex = (
+                numpy.bitwise_and(array.data > self.mosaic.data, ~array.mask)
+                | self.mosaic.mask
+            )
+
+            mask = numpy.where(pidex, array.mask, self.mosaic.mask)
+            self.mosaic = numpy.ma.where(pidex, array, self.mosaic)
+            self.mosaic.mask = mask
 
+
+@dataclass
 class LowestMethod(MosaicMethodBase):
-    """Feed the mosaic tile with the lowest pixel values."""
+    """Feed the mosaic array with the lowest pixel values."""
+
+    def feed(self, array: Optional[numpy.ma.MaskedArray]):
+        """Add data to the mosaic array."""
+        if self.mosaic is None:
+            self.mosaic = array
 
-    def feed(self, tile: Optional[numpy.ma.MaskedArray]):
-        """Add data to tile."""
-        if self.tile is None:
-            self.tile = tile
-
-        pidex = (
-            numpy.bitwise_and(tile.data < self.tile.data, ~tile.mask) | self.tile.mask
-        )
-
-        mask = numpy.where(pidex, tile.mask, self.tile.mask)
-        self.tile = numpy.ma.where(pidex, tile, self.tile)
-        self.tile.mask = mask
+        else:
+            pidex = (
+                numpy.bitwise_and(array.data < self.mosaic.data, ~array.mask)
+                | self.mosaic.mask
+            )
+
+            mask = numpy.where(pidex, array.mask, self.mosaic.mask)
+            self.mosaic = numpy.ma.where(pidex, array, self.mosaic)
+            self.mosaic.mask = mask
 
 
+@dataclass
 class MeanMethod(MosaicMethodBase):
-    """Stack the tiles and return the Mean pixel value."""
+    """Stack the arrays and return the Mean pixel value."""
 
-    def __init__(self, enforce_data_type: bool = True):
-        """Overwrite base and init Mean method."""
-        super(MeanMethod, self).__init__()
-        self.enforce_data_type = enforce_data_type
-        self.stack: List[numpy.ma.MaskedArray] = []
+    enforce_data_type: bool = True
+    stack: List[numpy.ma.MaskedArray] = field(default_factory=list, init=False)
 
     @property
-    def data(self) -> Tuple[Optional[numpy.ndarray], Optional[numpy.ndarray]]:
-        """Return data and mask."""
+    def data(self) -> Optional[numpy.ma.MaskedArray]:
+        """Return Mean of the data stack."""
         if self.stack:
-            tile = numpy.ma.mean(numpy.ma.stack(self.stack, axis=0), axis=0)
+            array = numpy.ma.mean(numpy.ma.stack(self.stack, axis=0), axis=0)
             if self.enforce_data_type:
-                tile = tile.astype(self.stack[0].dtype)
+                array = array.astype(self.stack[0].dtype)
 
-            data = numpy.ma.getdata(tile)
-            mask = ~numpy.logical_or.reduce(numpy.ma.getmaskarray(tile))
-            return (data, mask * numpy.uint8(255))
+            return array
 
-        else:
-            return None, None
+        return None
 
-    def feed(self, tile: Optional[numpy.ma.MaskedArray]):
-        """Add data to tile."""
-        self.stack.append(tile)
+    def feed(self, array: numpy.ma.MaskedArray):
+        """Add array to the stack."""
+        self.stack.append(array)
 
 
+@dataclass
 class MedianMethod(MosaicMethodBase):
-    """Stack the tiles and return the Median pixel value."""
+    """Stack the arrays and return the Median pixel value."""
 
-    def __init__(self, enforce_data_type: bool = True):
-        """Overwrite base and init Median method."""
-        super(MedianMethod, self).__init__()
-        self.enforce_data_type = enforce_data_type
-        self.stack: List[numpy.ma.MaskedArray] = []
+    enforce_data_type: bool = True
+    stack: List[numpy.ma.MaskedArray] = field(default_factory=list, init=False)
 
     @property
-    def data(self) -> Tuple[Optional[numpy.ndarray], Optional[numpy.ndarray]]:
-        """Return data and mask."""
+    def data(self) -> Optional[numpy.ma.MaskedArray]:
+        """Return Median of the data stack."""
         if self.stack:
-            tile = numpy.ma.median(numpy.ma.stack(self.stack, axis=0), axis=0)
+            array = numpy.ma.median(numpy.ma.stack(self.stack, axis=0), axis=0)
             if self.enforce_data_type:
-                tile = tile.astype(self.stack[0].dtype)
+                array = array.astype(self.stack[0].dtype)
 
-            data = numpy.ma.getdata(tile)
-            mask = ~numpy.logical_or.reduce(numpy.ma.getmaskarray(tile))
-            return (data, mask * numpy.uint8(255))
+            return array
 
-        else:
-            return None, None
+        return None
 
-    def feed(self, tile: Optional[numpy.ma.MaskedArray]):
-        """Create a stack of tile."""
-        self.stack.append(tile)
+    def feed(self, array: Optional[numpy.ma.MaskedArray]):
+        """Add array to the stack."""
+        self.stack.append(array)
 
 
+@dataclass
 class StdevMethod(MosaicMethodBase):
-    """Stack the tiles and return the Standard Deviation value."""
+    """Stack the arrays and return the Standard Deviation value."""
 
-    def __init__(self, enforce_data_type=True):
-        """Overwrite base and init Stdev method."""
-        super(StdevMethod, self).__init__()
-        self.stack: List[numpy.ma.MaskedArray] = []
+    stack: List[numpy.ma.MaskedArray] = field(default_factory=list, init=False)
 
     @property
-    def data(self) -> Tuple[Optional[numpy.ndarray], Optional[numpy.ndarray]]:
-        """Return data and mask."""
+    def data(self) -> Optional[numpy.ma.MaskedArray]:
+        """Return STDDEV of the data stack."""
         if self.stack:
-            tile = numpy.ma.std(numpy.ma.stack(self.stack, axis=0), axis=0)
+            return numpy.ma.std(numpy.ma.stack(self.stack, axis=0), axis=0)
 
-            data = numpy.ma.getdata(tile)
-            mask = ~numpy.logical_or.reduce(numpy.ma.getmaskarray(tile))
-            return (data, mask * numpy.uint8(255))
+        return None
 
-        else:
-            return None, None
-
-    def feed(self, tile: Optional[numpy.ma.MaskedArray]):
-        """Add data to tile."""
-        self.stack.append(tile)
+    def feed(self, array: Optional[numpy.ma.MaskedArray]):
+        """Add array to the stack."""
+        self.stack.append(array)
 
 
-class LastBandHigh(MosaicMethodBase):
-    """Feed the mosaic tile using the last band as decision factor."""
+@dataclass
+class LastBandHighMethod(MosaicMethodBase):
+    """Feed the mosaic array using the last band as decision factor (highest value)."""
 
     @property
-    def data(self) -> Tuple[Optional[numpy.ndarray], Optional[numpy.ndarray]]:
-        """Return data and mask."""
-        if self.tile is not None:
-            data = numpy.ma.getdata(self.tile)[:-1]
-            mask = ~numpy.logical_or.reduce(numpy.ma.getmaskarray(self.tile))
-            return (data, mask * numpy.uint8(255))
+    def data(self) -> Optional[numpy.ma.MaskedArray]:
+        """Return data."""
+        if self.mosaic is not None:
+            return self.mosaic[:-1].copy()
+
+        return None
+
+    def feed(self, array: Optional[numpy.ma.MaskedArray]):
+        """Add data to the mosaic array."""
+        if self.mosaic is None:
+            self.mosaic = array
 
         else:
-            return None, None
+            pidex = (
+                numpy.bitwise_and(array.data[-1] > self.mosaic.data[-1], ~array.mask)
+                | self.mosaic.mask
+            )
+
+            mask = numpy.where(pidex, array.mask, self.mosaic.mask)
+            self.mosaic = numpy.ma.where(pidex, array, self.mosaic)
+            self.mosaic.mask = mask
 
-    def feed(self, tile: Optional[numpy.ma.MaskedArray]):
-        """Add data to tile."""
-        if self.tile is None:
-            self.tile = tile
-            return
-
-        pidex = (
-            numpy.bitwise_and(tile.data[-1] > self.tile.data[-1], ~tile.mask)
-            | self.tile.mask
-        )
-
-        mask = numpy.where(pidex, tile.mask, self.tile.mask)
-        self.tile = numpy.ma.where(pidex, tile, self.tile)
-        self.tile.mask = mask
 
-
-class LastBandLow(MosaicMethodBase):
-    """Feed the mosaic tile using the last band as decision factor."""
+@dataclass
+class LastBandLowMethod(MosaicMethodBase):
+    """Feed the mosaic array using the last band as decision factor (lowest value)."""
 
     @property
-    def data(self) -> Tuple[Optional[numpy.ndarray], Optional[numpy.ndarray]]:
-        """Return data and mask."""
-        if self.tile is not None:
-            data = numpy.ma.getdata(self.tile)[:-1]
-            mask = ~numpy.logical_or.reduce(numpy.ma.getmaskarray(self.tile))
-            return (data, mask * numpy.uint8(255))
+    def data(self) -> Optional[numpy.ma.MaskedArray]:
+        """Return data."""
+        if self.mosaic is not None:
+            return self.mosaic[:-1].copy()
+
+        return None
+
+    def feed(self, array: Optional[numpy.ma.MaskedArray]):
+        """Add data to the mosaic array."""
+        if self.mosaic is None:
+            self.mosaic = array
 
         else:
-            return None, None
-
-    def feed(self, tile: Optional[numpy.ma.MaskedArray]):
-        """Add data to tile."""
-        if self.tile is None:
-            self.tile = tile
-            return
-
-        pidex = (
-            numpy.bitwise_and(tile.data[-1] < self.tile.data[-1], ~tile.mask)
-            | self.tile.mask
-        )
-
-        mask = numpy.where(pidex, tile.mask, self.tile.mask)
-        self.tile = numpy.ma.where(pidex, tile, self.tile)
-        self.tile.mask = mask
+            pidex = (
+                numpy.bitwise_and(array.data[-1] < self.mosaic.data[-1], ~array.mask)
+                | self.mosaic.mask
+            )
+
+            mask = numpy.where(pidex, array.mask, self.mosaic.mask)
+            self.mosaic = numpy.ma.where(pidex, array, self.mosaic)
+            self.mosaic.mask = mask
```

### Comparing `rio_tiler-4.1.9/.gitignore` & `rio_tiler-5.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/LICENSE` & `rio_tiler-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rio_tiler-4.1.9/README.md` & `rio_tiler-5.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   </a>
   <a href="https://anaconda.org/conda-forge/rio-tiler" target="_blank">
       <img src="https://img.shields.io/conda/v/conda-forge/rio-tiler.svg" alt="Conda Forge">
   </a>
   <a href="https://pypistats.org/packages/rio-tiler" target="_blank">
       <img src="https://img.shields.io/pypi/dm/rio-tiler.svg" alt="Downloads">
   </a>
-  <a href="https://github.com/cogeotiff/rio-tiler/blob/main/LICENSE.txt" target="_blank">
+  <a href="https://github.com/cogeotiff/rio-tiler/blob/main/LICENSE" target="_blank">
       <img src="https://img.shields.io/github/license/cogeotiff/rio-tiler.svg" alt="Downloads">
   </a>
   <a href="https://mybinder.org/v2/gh/cogeotiff/rio-tiler/main?filepath=docs%2Fexamples%2F" target="_blank" alt="Binder">
       <img src="https://mybinder.org/badge_logo.svg" alt="Binder">
   </a>
 </p>
 
@@ -194,21 +194,18 @@
 
 Create Mapbox Vector Tiles from raster sources
 
 [rio-tiler-mvt]: https://github.com/cogeotiff/rio-tiler-mvt
 
 ## Implementations
 
-[**rio-viz**][rio-viz]: Visualize Cloud Optimized GeoTIFFs locally in the browser
-
 [**titiler**][titiler]: A lightweight Cloud Optimized GeoTIFF dynamic tile server.
 
 [**cogeo-mosaic**][cogeo-mosaic]: Create mosaics of Cloud Optimized GeoTIFF based on the [mosaicJSON][mosaicjson_spec] specification.
 
-[rio-viz]: https://github.com/developmentseed/rio-viz
 [titiler]: https://github.com/developmentseed/titiler
 [cogeo-mosaic]: https://github.com/developmentseed/cogeo-mosaic
 [mosaicjson_spec]: https://github.com/developmentseed/mosaicjson-spec
 
 ## Contribution & Development
 
 See [CONTRIBUTING.md](https://github.com/cogeotiff/rio-tiler/blob/main/CONTRIBUTING.md)
```

### Comparing `rio_tiler-4.1.9/pyproject.toml` & `rio_tiler-5.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,19 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = ["version"]
 dependencies = [
     "attrs",
-    "boto3",
     "cachetools",
     "httpx",
     "numexpr",
     "numpy",
-    "morecantile>=3.1,<4.0",
+    "morecantile>=4.0,<5.0",
     "pydantic",
     "pystac>=0.5.4",
     "rasterio>=1.3.0",
     "color-operations",
     "importlib_resources>=1.1.0; python_version < '3.9'",
 ]
 
@@ -40,18 +39,23 @@
     "pytest-asyncio",
     "pytest-benchmark",
     "pytest-cov",
 
     # XarrayReader
     "xarray",
     "rioxarray",
+    # S3
+    "boto3",
 ]
 dev = [
     "pre-commit",
 ]
+s3 = [
+    "boto3",
+]
 xarray = [
     "xarray",
     "rioxarray",
 ]
 docs = [
     "nbconvert",
     "mkdocs",
@@ -116,14 +120,15 @@
 no_strict_optional = true
 
 [tool.ruff]
 select = [
     "D1",  # pydocstyle errors
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
+    "F",  # flake8
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
 ]
 ignore = [
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
     "B905",  # ignore zip() without an explicit strict= parameter, only support with python >3.10
```

### Comparing `rio_tiler-4.1.9/PKG-INFO` & `rio_tiler-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rio-tiler
-Version: 4.1.9
+Version: 5.0.0
 Summary: User friendly Rasterio plugin to read raster datasets.
 Project-URL: Homepage, https://cogeotiff.github.io/rio-tiler/
 Project-URL: Documentation, https://cogeotiff.github.io/rio-tiler/
 Project-URL: Issues, https://github.com/cogeotiff/rio-tiler/issues
 Project-URL: Source, https://github.com/cogeotiff/rio-tiler
 Project-URL: Changelog, https://cogeotiff.github.io/rio-tiler/release-notes/
 Author-email: Vincent Sarago <vincent@developmentseed.com>
@@ -46,34 +46,36 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Requires-Dist: attrs
-Requires-Dist: boto3
 Requires-Dist: cachetools
 Requires-Dist: color-operations
 Requires-Dist: httpx
 Requires-Dist: importlib-resources>=1.1.0; python_version < '3.9'
-Requires-Dist: morecantile<4.0,>=3.1
+Requires-Dist: morecantile<5.0,>=4.0
 Requires-Dist: numexpr
 Requires-Dist: numpy
 Requires-Dist: pydantic
 Requires-Dist: pystac>=0.5.4
 Requires-Dist: rasterio>=1.3.0
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == 'docs'
 Requires-Dist: mkdocs-jupyter; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: nbconvert; extra == 'docs'
 Requires-Dist: pygments; extra == 'docs'
+Provides-Extra: s3
+Requires-Dist: boto3; extra == 's3'
 Provides-Extra: test
+Requires-Dist: boto3; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-benchmark; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: rioxarray; extra == 'test'
 Requires-Dist: xarray; extra == 'test'
 Provides-Extra: xarray
@@ -101,15 +103,15 @@
   </a>
   <a href="https://anaconda.org/conda-forge/rio-tiler" target="_blank">
       <img src="https://img.shields.io/conda/v/conda-forge/rio-tiler.svg" alt="Conda Forge">
   </a>
   <a href="https://pypistats.org/packages/rio-tiler" target="_blank">
       <img src="https://img.shields.io/pypi/dm/rio-tiler.svg" alt="Downloads">
   </a>
-  <a href="https://github.com/cogeotiff/rio-tiler/blob/main/LICENSE.txt" target="_blank">
+  <a href="https://github.com/cogeotiff/rio-tiler/blob/main/LICENSE" target="_blank">
       <img src="https://img.shields.io/github/license/cogeotiff/rio-tiler.svg" alt="Downloads">
   </a>
   <a href="https://mybinder.org/v2/gh/cogeotiff/rio-tiler/main?filepath=docs%2Fexamples%2F" target="_blank" alt="Binder">
       <img src="https://mybinder.org/badge_logo.svg" alt="Binder">
   </a>
 </p>
 
@@ -277,21 +279,18 @@
 
 Create Mapbox Vector Tiles from raster sources
 
 [rio-tiler-mvt]: https://github.com/cogeotiff/rio-tiler-mvt
 
 ## Implementations
 
-[**rio-viz**][rio-viz]: Visualize Cloud Optimized GeoTIFFs locally in the browser
-
 [**titiler**][titiler]: A lightweight Cloud Optimized GeoTIFF dynamic tile server.
 
 [**cogeo-mosaic**][cogeo-mosaic]: Create mosaics of Cloud Optimized GeoTIFF based on the [mosaicJSON][mosaicjson_spec] specification.
 
-[rio-viz]: https://github.com/developmentseed/rio-viz
 [titiler]: https://github.com/developmentseed/titiler
 [cogeo-mosaic]: https://github.com/developmentseed/cogeo-mosaic
 [mosaicjson_spec]: https://github.com/developmentseed/mosaicjson-spec
 
 ## Contribution & Development
 
 See [CONTRIBUTING.md](https://github.com/cogeotiff/rio-tiler/blob/main/CONTRIBUTING.md)
```

