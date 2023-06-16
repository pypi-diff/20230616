# Comparing `tmp/spagrn-1.0.4.tar.gz` & `tmp/spagrn-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spagrn-1.0.4.tar", last modified: Sun Apr 23 11:07:13 2023, max compression
+gzip compressed data, was "dist/spagrn-1.0.5.tar", last modified: Fri Jun 16 00:51:45 2023, max compression
```

## Comparing `spagrn-1.0.4.tar` & `spagrn-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yao        (502) staff       (20)        0 2023-04-23 11:07:13.822382 spagrn-1.0.4/
--rw-r--r--   0 yao        (502) staff       (20)    35149 2023-04-11 12:27:22.000000 spagrn-1.0.4/LICENSE
--rw-r--r--   0 yao        (502) staff       (20)      627 2023-04-23 11:07:13.822441 spagrn-1.0.4/PKG-INFO
--rw-r--r--   0 yao        (502) staff       (20)     3617 2023-04-23 10:09:19.000000 spagrn-1.0.4/README.md
--rw-r--r--   0 yao        (502) staff       (20)       79 2023-04-23 11:07:13.822647 spagrn-1.0.4/setup.cfg
--rw-r--r--   0 yao        (502) staff       (20)     1207 2023-04-23 11:06:44.000000 spagrn-1.0.4/setup.py
-drwxr-xr-x   0 yao        (502) staff       (20)        0 2023-04-23 11:07:13.821684 spagrn-1.0.4/spagrn/
--rw-r--r--   0 yao        (502) staff       (20)      282 2023-04-21 12:16:13.000000 spagrn-1.0.4/spagrn/__init__.py
--rw-r--r--   0 yao        (502) staff       (20)    13782 2023-04-21 12:16:13.000000 spagrn-1.0.4/spagrn/plot.py
--rw-r--r--   0 yao        (502) staff       (20)    39463 2023-04-21 12:16:13.000000 spagrn-1.0.4/spagrn/regulatory_network.py
--rw-r--r--   0 yao        (502) staff       (20)     1202 2023-04-08 12:20:26.000000 spagrn-1.0.4/spagrn/spa_logger.py
--rw-r--r--   0 yao        (502) staff       (20)     1867 2023-04-08 12:23:27.000000 spagrn-1.0.4/spagrn/test.py
-drwxr-xr-x   0 yao        (502) staff       (20)        0 2023-04-23 11:07:13.822296 spagrn-1.0.4/spagrn.egg-info/
--rw-r--r--   0 yao        (502) staff       (20)      627 2023-04-23 11:07:13.000000 spagrn-1.0.4/spagrn.egg-info/PKG-INFO
--rw-r--r--   0 yao        (502) staff       (20)      284 2023-04-23 11:07:13.000000 spagrn-1.0.4/spagrn.egg-info/SOURCES.txt
--rw-r--r--   0 yao        (502) staff       (20)        1 2023-04-23 11:07:13.000000 spagrn-1.0.4/spagrn.egg-info/dependency_links.txt
--rw-r--r--   0 yao        (502) staff       (20)      143 2023-04-23 11:07:13.000000 spagrn-1.0.4/spagrn.egg-info/requires.txt
--rw-r--r--   0 yao        (502) staff       (20)        7 2023-04-23 11:07:13.000000 spagrn-1.0.4/spagrn.egg-info/top_level.txt
+drwxr-xr-x   0 Oreo       (501) staff       (20)        0 2023-06-16 00:51:45.000000 spagrn-1.0.5/
+-rw-r--r--   0 Oreo       (501) staff       (20)    35149 2023-04-12 05:49:34.000000 spagrn-1.0.5/LICENSE
+-rw-r--r--   0 Oreo       (501) staff       (20)      617 2023-06-16 00:51:45.000000 spagrn-1.0.5/PKG-INFO
+-rw-r--r--   0 Oreo       (501) staff       (20)     3846 2023-05-25 10:13:51.000000 spagrn-1.0.5/README.md
+-rw-r--r--   0 Oreo       (501) staff       (20)       79 2023-06-16 00:51:45.000000 spagrn-1.0.5/setup.cfg
+-rw-r--r--   0 Oreo       (501) staff       (20)     1222 2023-05-25 10:13:51.000000 spagrn-1.0.5/setup.py
+drwxr-xr-x   0 Oreo       (501) staff       (20)        0 2023-06-16 00:51:45.000000 spagrn-1.0.5/spagrn/
+-rw-r--r--   0 Oreo       (501) staff       (20)      746 2023-05-26 05:52:44.000000 spagrn-1.0.5/spagrn/__init__.py
+-rw-r--r--   0 Oreo       (501) staff       (20)    11399 2023-06-16 00:51:09.000000 spagrn-1.0.5/spagrn/plot.py
+-rw-r--r--   0 Oreo       (501) staff       (20)    39894 2023-05-26 03:27:47.000000 spagrn-1.0.5/spagrn/regulatory_network.py
+-rw-r--r--   0 Oreo       (501) staff       (20)     1202 2023-04-09 04:47:05.000000 spagrn-1.0.5/spagrn/spa_logger.py
+-rw-r--r--   0 Oreo       (501) staff       (20)     1815 2023-05-26 03:31:09.000000 spagrn-1.0.5/spagrn/test.py
+drwxr-xr-x   0 Oreo       (501) staff       (20)        0 2023-06-16 00:51:45.000000 spagrn-1.0.5/spagrn.egg-info/
+-rw-r--r--   0 Oreo       (501) staff       (20)      617 2023-06-16 00:51:45.000000 spagrn-1.0.5/spagrn.egg-info/PKG-INFO
+-rw-r--r--   0 Oreo       (501) staff       (20)      284 2023-06-16 00:51:45.000000 spagrn-1.0.5/spagrn.egg-info/SOURCES.txt
+-rw-r--r--   0 Oreo       (501) staff       (20)        1 2023-06-16 00:51:45.000000 spagrn-1.0.5/spagrn.egg-info/dependency_links.txt
+-rw-r--r--   0 Oreo       (501) staff       (20)      157 2023-06-16 00:51:45.000000 spagrn-1.0.5/spagrn.egg-info/requires.txt
+-rw-r--r--   0 Oreo       (501) staff       (20)        7 2023-06-16 00:51:45.000000 spagrn-1.0.5/spagrn.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `spagrn-1.0.4/LICENSE` & `spagrn-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spagrn-1.0.4/PKG-INFO` & `spagrn-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: spagrn
-Version: 1.0.4
+Version: 1.0.5
 Summary: A comprehensive tool to infer TF-centered, spatial gene regulatory networks for the spatially resolved transcriptomic data.
 Home-page: https://github.com/BGI-Qingdao/SpaGRN
 Author: Yao LI, Lidong GUO, Mengyang XU
 Author-email: liyao1@genomics.cn, guolidong@genomics.cn, xumengyang@genomics.cn
 License: GPL-3.0+
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.11
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `spagrn-1.0.4/README.md` & `spagrn-1.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,39 +17,50 @@
 
 All input SRT data and related TF database can be inquired or directly downloaded from http://www.bgiocean.com/SpaGRN/
 We also provide an interactive 3D GRN atlas database, covering different GRN inference tools for different SRT datasets generated by different SRT sequencing platforms (http://www.bgiocean.com/SpaGRN/). 
 
 
 # Installation
 To install the latest version of SpaGRN via `PyPI`:
-```å
-pip install spagrn
 ```
+pip install spagrn==1.0.4
+```
+Or install by bioconda
+
+```
+conda install -c bioconda spagrn
+
+# Notice: If you install via conda, you will need to install the following dependencies separately:
+#pyscenic==0.12.1
+#hotspotsc==1.1.1
+#arboreto
+#ctxcore>=0.2.0
+```
+
 SpaGRN can be imported as:
 ```
 from spagrn import InferRegulatoryNetwork as irn
 from spagrn import PlotRegulatoryNetwork as prn
 ```
 
-Dependencies
+Dependencies:
 ```
-anndata==0.8.0 
-pandas>=1.3.5
-scanpy
+anndata==0.8.0
+pandas<2.0.0,>=1.3.4
+scanpy==1.9.1
 seaborn
 matplotlib 
 pyscenic==0.12.1
 hotspotsc==1.1.1
 scipy
 numpy
 dask
 arboreto
 ctxcore>=0.2.0
-sklearn
-multiprocessing_on_dill
+scikit-learn
 ```
 
 
 # Usage
 The package provides functions for loading data, preprocessing data, reconstructing gene network, and visualizing the inferred GRNs. The main functions are:
 * Load and process data
 * Compute TF-gene similarities
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spagrn-1.0.4/setup.py` & `spagrn-1.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import setuptools
 import glob
 import os
 from pathlib import Path
 
 setuptools.setup(
     name="spagrn",
-    version="1.0.4",
+    version="1.0.5",
     author="Yao LI, Lidong GUO, Mengyang XU",
     author_email="liyao1@genomics.cn, guolidong@genomics.cn, xumengyang@genomics.cn",
     url="https://github.com/BGI-Qingdao/SpaGRN",
     #long_description=Path('README.md').read_text('utf-8'),
     python_requires=">=3.7,<3.11",
     packages=setuptools.find_packages(),
     install_requires=[
         "anndata==0.8.0",
-        "pandas>=1.3.5",
-        "scanpy",
+        "pandas<2.0.0, >=1.3.4",
+        "scanpy==1.9.1",
         "seaborn",
         "matplotlib",
         "pyscenic==0.12.1",
         "hotspotsc==1.1.1",
         "scipy",
         #"numpy<1.20.0,>=1.16.6",
         "numpy",
```

### Comparing `spagrn-1.0.4/spagrn/plot.py` & `spagrn-1.0.5/spagrn/plot.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,404 +11,341 @@
 change log:
     2023/01/08 init
 """
 
 # python core modules
 
 # third party modules
-from typing import Union
-
 import anndata
-import logging
 import pandas as pd
 import numpy as np
 import scanpy as sc
 import seaborn as sns
 import matplotlib.pyplot as plt
-from pyscenic.cli.utils import load_signatures
-from pyscenic.export import add_scenic_metadata
 from pyscenic.rss import regulon_specificity_scores
 import matplotlib as mpl
 
 mpl.rcParams['pdf.fonttype'] = 42
 mpl.rcParams['ps.fonttype'] = 42
 mpl.rcParams['svg.fonttype'] = 'none'
 mpl.rcParams["ytick.labelright"] = True
 mpl.rcParams["ytick.labelleft"] = False
 
 # modules in self project
 
-logger = logging.getLogger()
+
+################################################
+#                                              #
+#        Plot Gene Regulatory Networks         #
+#                                              #
+################################################
+COLORS = [
+    '#d60000', '#e2afaf', '#018700', '#a17569', '#e6a500', '#004b00',
+    '#6b004f', '#573b00', '#005659', '#5e7b87', '#0000dd', '#00acc6',
+    '#bcb6ff', '#bf03b8', '#645472', '#790000', '#0774d8', '#729a7c',
+    '#8287ff', '#ff7ed1', '#8e7b01', '#9e4b00', '#8eba00', '#a57bb8',
+    '#5901a3', '#8c3bff', '#a03a52', '#a1c8c8', '#f2007b', '#ff7752',
+    '#bac389', '#15e18c', '#60383b', '#546744', '#380000', '#e252ff',
+]
+
+
+# dotplot method for anndata
+def dotplot_anndata(data: anndata.AnnData,
+                    gene_names: list,
+                    cluster_label: str,
+                    save: bool = True,
+                    **kwargs):
+    """
+    create a dotplot for Anndata object.
+    a dotplot contains percent (of cells that) expressed (the genes) and average expression (of genes).
+
+    :param data: gene data
+    :param gene_names: interested gene names
+    :param cluster_label: label of clustering output
+    :param save: if save plot into a file
+    :param kwargs: features Input vector of features, or named list of feature vectors
+    if feature-grouped panels are desired
+    :return: plt axe object
+    """
+    if isinstance(data, anndata.AnnData):
+        return sc.pl.dotplot(data, var_names=gene_names, groupby=cluster_label, save=save, **kwargs)
 
 
-class PlotRegulatoryNetwork:
+def plot_2d_reg(data: anndata.AnnData,
+                pos_label,
+                auc_mtx,
+                reg_name: str,
+                fn: str,
+                **kwargs):
     """
-    Plot Gene Regulatory Networks related plots
+    Plot genes of one regulon on a 2D map
+    :param pos_label:
+    :param data:
+    :param auc_mtx:
+    :param reg_name:
+    :param fn:
+    :return:
     """
+    if '(+)' not in reg_name:
+        reg_name = reg_name + '(+)'
 
-    def __init__(self, data, cluster_label='annotation'):
-        self._data = data
-        self._regulon_list = None
-        self._auc_mtx = None
-        self._regulon_dict = None
-
-        self._celltype_colors = [
-            '#d60000', '#e2afaf', '#018700', '#a17569', '#e6a500', '#004b00',
-            '#6b004f', '#573b00', '#005659', '#5e7b87', '#0000dd', '#00acc6',
-            '#bcb6ff', '#bf03b8', '#645472', '#790000', '#0774d8', '#729a7c',
-            '#8287ff', '#ff7ed1', '#8e7b01', '#9e4b00', '#8eba00', '#a57bb8',
-            '#5901a3', '#8c3bff', '#a03a52', '#a1c8c8', '#f2007b', '#ff7752',
-            '#bac389', '#15e18c', '#60383b', '#546744', '#380000', '#e252ff',
-        ]
-        self._cluster_label = cluster_label
-
-    @property
-    def data(self):
-        return self._data
-
-    @data.setter
-    def data(self, value):
-        self._data = value
-
-    @property
-    def regulon_list(self):
-        return self._regulon_list
-
-    @regulon_list.setter
-    def regulon_list(self, value):
-        self._regulon_list = value
-
-    @property
-    def regulon_dict(self):
-        return self._regulon_dict
-
-    @regulon_dict.setter
-    def regulon_dict(self, value):
-        self._regulon_dict = value
-
-    @property
-    def auc_mtx(self):
-        return self._auc_mtx
-
-    @auc_mtx.setter
-    def auc_mtx(self, value):
-        self._auc_mtx = value
-
-    @property
-    def celltype_colors(self):
-        return self._celltype_colors
-
-    @celltype_colors.setter
-    def celltype_colors(self, value):
-        self._celltype_colors = value
-
-    @property
-    def cluster_label(self):
-        return self._cluster_label
-
-    @cluster_label.setter
-    def cluster_label(self, value):
-        self._cluster_label = value
-
-    def add_color(self, value):
-        if isinstance(value, list):
-            self._celltype_colors.extend(value)
-        elif isinstance(value, str):
-            self._celltype_colors.append(value)
-        else:
-            logger.error('new color should be either a string or a list of strings')
-
-    # dotplot method for anndata
-    @staticmethod
-    def dotplot_anndata(data: anndata.AnnData,
-                        gene_names: list,
-                        cluster_label: str,
-                        save: bool = True,
-                        **kwargs):
-        """
-        create a dotplot for Anndata object.
-        a dotplot contains percent (of cells that) expressed (the genes) and average expression (of genes).
-
-        :param data: gene data
-        :param gene_names: interested gene names
-        :param cluster_label: label of clustering output
-        :param save: if save plot into a file
-        :param kwargs: features Input vector of features, or named list of feature vectors
-        if feature-grouped panels are desired
-        :return: plt axe object
-        """
-        if isinstance(data, anndata.AnnData):
-            return sc.pl.dotplot(data, var_names=gene_names, groupby=cluster_label, save=save, **kwargs)
-
-    @staticmethod
-    def plot_2d_reg(data: anndata.AnnData,
-                    pos_label,
-                    auc_mtx,
-                    reg_name: str,
-                    fn: str,
-                    **kwargs):
-        """
-        Plot genes of one regulon on a 2D map
-        :param pos_label:
-        :param data:
-        :param auc_mtx:
-        :param reg_name:
-        :param fn:
-        :return:
-        """
-        if '(+)' not in reg_name:
-            reg_name = reg_name + '(+)'
-        if fn is None:
-            fn = f'{reg_name.strip("(+)")}.pdf'
-
-        cell_coor = data.obsm[pos_label]
-        auc_zscore = PlotRegulatoryNetwork.cal_zscore(auc_mtx)
-        # prepare plotting data
-        sub_zscore = auc_zscore[reg_name]
-        # sort data points by zscore (low to high), because first dot will be covered by latter dots
-        zorder = np.argsort(sub_zscore.values)
-        # plot cell/bin dot, x y coor
-        sc = plt.scatter(cell_coor[:, 0][zorder],
-                         cell_coor[:, 1][zorder],
-                         c=sub_zscore.iloc[zorder],
-                         marker='.',
-                         edgecolors='none',
-                         cmap='plasma',
-                         lw=0,
-                         **kwargs)
-        plt.axis("equal")
-        plt.box(False)
-        plt.axis('off')
-        plt.colorbar(sc, shrink=0.35)
-        plt.savefig(fn, format='pdf')
-        plt.close()
-
-    @staticmethod
-    def plot_3d_reg(data: anndata.AnnData,
-                    pos_label,
-                    auc_mtx,
-                    reg_name: str,
-                    fn: str,
-                    view_vertical=222,
-                    view_horizontal=-80,
-                    **kwargs):
-        """
-        Plot genes of one regulon on a 3D map
-        :param pos_label:
-        :param data:
-        :param auc_mtx:
-        :param reg_name:
-        :param fn:
-        :param view_vertical: vertical angle to view to the 3D object
-        :param view_horizontal: horizontal angle to view the 3D object
-        :return:
-
-        Example:
-            plot_3d_reg(data, 'spatial', auc_mtx, 'Zfp354c', view_vertical=30, view_horizontal=-30)
-        """
-        if '(+)' not in reg_name:
-            reg_name = reg_name + '(+)'
-        if fn is None:
-            fn = f'{reg_name.strip("(+)")}.pdf'
-
-        # prepare plotting data
-        cell_coor = data.obsm[pos_label]
-        auc_zscore = PlotRegulatoryNetwork.cal_zscore(auc_mtx)
-        sub_zscore = auc_zscore[reg_name]
-
-        from mpl_toolkits.mplot3d import Axes3D
-        fig = plt.figure()
-        ax = Axes3D(fig)
-        sc = ax.scatter(cell_coor[:, 0],
-                        cell_coor[:, 1],
-                        cell_coor[:, 2],
-                        c=sub_zscore,
-                        marker='.',
-                        edgecolors='none',
-                        cmap='plasma',
-                        lw=0, **kwargs)
-        # set view angle
-        ax.view_init(view_vertical, view_horizontal)
-        # scale axis
-        xlen = cell_coor[:, 0].max() - cell_coor[:, 0].min()
-        ylen = cell_coor[:, 1].max() - cell_coor[:, 1].min()
-        zlen = cell_coor[:, 2].max() - cell_coor[:, 2].min()
-        yscale = ylen / xlen
-        zscale = zlen / xlen
-        ax.get_proj = lambda: np.dot(Axes3D.get_proj(ax), np.diag([1, yscale, zscale, 1]))
+    cell_coor = data.obsm[pos_label]
+    auc_zscore = cal_zscore(auc_mtx)
+    # prepare plotting data
+    sub_zscore = auc_zscore[reg_name]
+    # sort data points by zscore (low to high), because first dot will be covered by latter dots
+    zorder = np.argsort(sub_zscore.values)
+    # plot cell/bin dot, x y coor
+    sc = plt.scatter(cell_coor[:, 0][zorder],
+                     cell_coor[:, 1][zorder],
+                     c=sub_zscore.iloc[zorder],
+                     marker='.',
+                     edgecolors='none',
+                     cmap='plasma',
+                     lw=0,
+                     **kwargs)
+    plt.axis("equal")
+    plt.box(False)
+    plt.axis('off')
+    plt.colorbar(sc, shrink=0.35)
+    plt.savefig(fn, format='pdf')
+    plt.close()
+
+
+def plot_3d_reg(data: anndata.AnnData,
+                pos_label,
+                auc_mtx,
+                reg_name: str,
+                fn: str,
+                view_vertical=222,
+                view_horizontal=-80,
+                show_bg=False,
+                xscale=1,
+                yscale=1,
+                zscale=1,
+                **kwargs):
+    """
+    Plot genes of one regulon on a 3D map
+    :param pos_label:
+    :param data:
+    :param auc_mtx:
+    :param reg_name:
+    :param fn:
+    :param view_vertical: vertical angle to view to the 3D object
+    :param view_horizontal: horizontal angle to view the 3D object
+    :param show_bg: if show background
+    :param xscale:
+    :param yscale:
+    :param zscale:
+    :return:
+
+    Example:
+        plot_3d_reg(data, 'spatial', auc_mtx, 'Zfp354c', view_vertical=30, view_horizontal=-30)
+    """
+    if '(+)' not in reg_name:
+        reg_name = reg_name + '(+)'
 
+    # prepare plotting data
+    cell_coor = data.obsm[pos_label]
+    auc_zscore = cal_zscore(auc_mtx)
+    sub_zscore = auc_zscore[reg_name]
+
+    from mpl_toolkits.mplot3d import Axes3D
+    fig = plt.figure()
+    ax = Axes3D(fig)
+    sc = ax.scatter(cell_coor[:, 0],
+                    cell_coor[:, 1],
+                    cell_coor[:, 2],
+                    c=sub_zscore,
+                    marker='.',
+                    edgecolors='none',
+                    cmap='plasma',
+                    lw=0, **kwargs)
+    # set view angle
+    ax.view_init(view_vertical, view_horizontal)
+    # scale axis
+    xlen = cell_coor[:, 0].max() - cell_coor[:, 0].min()
+    ylen = cell_coor[:, 1].max() - cell_coor[:, 1].min()
+    zlen = cell_coor[:, 2].max() - cell_coor[:, 2].min()
+    _xscale = xscale
+    _yscale = ylen / xlen * yscale
+    _zscale = zlen / xlen * zscale
+    ax.get_proj = lambda: np.dot(Axes3D.get_proj(ax), np.diag([_xscale, _yscale, _zscale, 1]))
+
+    if not show_bg:
         plt.box(False)
         plt.axis('off')
-        plt.colorbar(sc, shrink=0.35)
-        plt.savefig(fn, format='pdf')
-        plt.close()
-
-    @staticmethod
-    def rss_heatmap(data: anndata.AnnData,
-                    auc_mtx: pd.DataFrame,
-                    cluster_label: str,
-                    rss_fn: str = 'regulon_specificity_scores.txt',
-                    topn=5,
-                    save=True,
-                    subset=True,
-                    subset_size=5000, 
-                    fn='clusters_heatmap_top5.pdf',
-                    legend_fn="rss_celltype_legend_top5.png"):
-        """
-        Plot heatmap for Regulon specificity scores (RSS) value
-        :param data: 
-        :param auc_mtx: 
-        :param cluster_label:
-        :param rss_fn:
-        :param topn:
-        :param save:
-        :param subset:
-        :parma subset_size:
-        :param fn:
-        :return:
-        """
-        if subset and len(data.obs) > subset_size:
-            fraction = subset_size / len(data.obs)
-            #do stratified sampling
-            draw_obs = data.obs.groupby(cluster_label, group_keys=False).apply(lambda x: x.sample(frac=fraction))
-            # load the regulon_list from a file using the load_signatures function
-            cell_order = draw_obs[cluster_label].sort_values()
-        else:
-            # load the regulon_list from a file using the load_signatures function
-            cell_order = data.obs[cluster_label].sort_values()
-        celltypes = sorted(list(set(data.obs[cluster_label])))
+    plt.colorbar(sc, shrink=0.35)
+    plt.savefig(fn)
+    plt.close()
+
+
+def rss_heatmap(data: anndata.AnnData,
+                auc_mtx: pd.DataFrame,
+                cluster_label: str,
+                rss_fn: str,
+                topn=5,
+                save=True,
+                subset=True,
+                subset_size=5000,
+                fn='clusters_heatmap_top5.png',
+                legend_fn="rss_celltype_legend.png",
+                cluster_list=None):
+    """
+    Plot heatmap for Regulon specificity scores (RSS) value
+    :param data:
+    :param auc_mtx:
+    :param cluster_label:
+    :param rss_fn:
+    :param topn:
+    :param save:
+    :param subset:
+    :param subset_size:
+    :param fn:
+    :param legend_fn:
+    :param cluster_list: list of cluster names one prefer to use
+    :return:
 
-        # Regulon specificity scores (RSS) across predicted cell types
+    Example:
+        # only plot ['CNS', 'amnioserosa', 'carcass'] clusters and their corresponding top regulons
+        rss_heatmap(adata, auc_mtx, cluster_label='celltypes', subset=False,
+                    rss_fn='regulon_specificity_scores.txt',
+                    cluster_list=['CNS', 'amnioserosa', 'carcass'])
+    """
+    if subset and len(data.obs) > subset_size:
+        fraction = subset_size / len(data.obs)
+        # do stratified sampling
+        draw_obs = data.obs.groupby(cluster_label, group_keys=False).apply(lambda x: x.sample(frac=fraction))
+        # load the regulon_list from a file using the load_signatures function
+        cell_order = draw_obs[cluster_label].sort_values()
+    else:
+        # load the regulon_list from a file using the load_signatures function
+        cell_order = data.obs[cluster_label].sort_values()
+    celltypes = sorted(list(set(data.obs[cluster_label])))
+
+    # Regulon specificity scores (RSS) across predicted cell types
+    if rss_fn is None:
+        rss_cellType = regulon_specificity_scores(auc_mtx, data.obs[cluster_label])
+    else:
         rss_cellType = pd.read_csv(rss_fn, index_col=0)
-        # Select the top 5 regulon_list from each cell type
-        topreg = PlotRegulatoryNetwork.get_top_regulons(data, cluster_label, rss_cellType, topn=topn)
+    # Select the top 5 regulon_list from each cell type
+    topreg = get_top_regulons(data, cluster_label, rss_cellType, topn=topn)
 
+    if cluster_list is None:
+        cluster_list = celltypes.copy()
+    colorsd = dict((i, c) for i, c in zip(cluster_list, COLORS))
+    colormap = [colorsd[x] for x in cell_order]
 
-        obs_list = ['CNS', 'amnioserosa', 'carcass', 'epidermis', 'epidermis/CNS', 'fat body', 'fat body/trachea', 'foregut', 'foregut/garland cells', 'hemolymph', 'hindgut', 'hindgut/malpighian tubule', 'midgut', 'midgut/malpighian tubules', 'muscle', 'salivary gland', 'testis', 'trachea']
+    # plot legend
+    plot_legend(colorsd, legend_fn)
 
-        colors = [
-            '#d60000', '#e2afaf', '#018700', '#a17569', '#e6a500', '#004b00',
-            '#6b004f', '#573b00', '#005659', '#5e7b87', '#0000dd', '#00acc6',
-            '#bcb6ff', '#bf03b8', '#645472', '#790000', '#0774d8', '#729a7c',
-            '#8287ff', '#ff7ed1', '#8e7b01', '#9e4b00', '#8eba00', '#a57bb8',
-            '#5901a3', '#8c3bff', '#a03a52', '#a1c8c8', '#f2007b', '#ff7752',
-            '#bac389', '#15e18c', '#60383b', '#546744', '#380000', '#e252ff',
-        ]
-        colorsd = dict((i, c) for i, c in zip(obs_list, colors))
-        colormap = [colorsd[x] for x in cell_order]        
-
-        # plot legend
-        #plot_legend(colormap, obs_list, legend_fn)
-
-        # plot z-score
-        auc_zscore = PlotRegulatoryNetwork.cal_zscore(auc_mtx)
-        plot_data = auc_zscore[topreg].loc[cell_order.index]
-        sns.set(font_scale=1.2)
-        g = sns.clustermap(plot_data,
-                           annot=False,
-                           square=False,
-                           linecolor='gray',
-                           yticklabels=True, xticklabels=True,
-                           vmin=-3, vmax=3,
-                           cmap="YlGnBu",
-                           row_colors=colormap,
-                           row_cluster=False, col_cluster=True)
-        g.cax.set_visible(True)
-        g.ax_heatmap.set_yticks([])
-        g.ax_heatmap.set_ylabel('')
-        g.ax_heatmap.set_xlabel('')
-        if save:
-            plt.savefig(fn, format='pdf')
-        return g
-
-    @staticmethod
-    def map_celltype_colors(data, celltype_colors: list, celltypes: list, cluster_label: str):
-        """
-
-        :param data:
-        :param celltype_colors:
-        :param celltypes:
-        :param cluster_label:
-        :return:
-        """
-        assert len(celltype_colors) >= len(celltypes)
-        colorsd = dict((i, c) for i, c in zip(celltypes, celltype_colors))
-        colormap = [colorsd[x] for x in data.obs[cluster_label]]
-        return colorsd, colormap
-
-    @staticmethod
-    def get_top_regulons(data: anndata.AnnData, cluster_label: str, rss_celltype: pd.DataFrame, topn: int) -> list:
-        """
-        get top n regulons for each cell type based on regulon specificity scores (rss)
-        :param data:
-        :param cluster_label:
-        :param rss_celltype:
-        :param topn:
-        :return: a list
-        """
-        # Select the top 5 regulon_list from each cell type
-        cats = sorted(list(set(data.obs[cluster_label])))
-        topreg = []
-        for i, c in enumerate(cats):
-            topreg.extend(
-                list(rss_celltype.T[c].sort_values(ascending=False)[:topn].index)
-            )
-        topreg = list(set(topreg))
-        return topreg
-
-    @staticmethod
-    def cal_zscore(auc_mtx: pd.DataFrame, save=False) -> pd.DataFrame:
-        """
-        calculate z-score for each gene among cells
-        :param auc_mtx:
-        :param save:
-        :return:
-        """
-        func = lambda x: (x - x.mean()) / x.std(ddof=0)
-        auc_zscore = auc_mtx.transform(func, axis=0)
-        if save:
-            auc_zscore.to_csv('auc_zscore.csv', index=False)
-        return auc_zscore
+    # plot z-score
+    auc_zscore = cal_zscore(auc_mtx)
+    plot_data = auc_zscore[topreg].loc[cell_order.index]
+    sns.set(font_scale=1.2)
+    g = sns.clustermap(plot_data,
+                       annot=False,
+                       square=False,
+                       linecolor='gray',
+                       yticklabels=True, xticklabels=True,
+                       vmin=-3, vmax=3,
+                       cmap="YlGnBu",
+                       row_colors=colormap,
+                       row_cluster=False, col_cluster=True)
+    g.cax.set_visible(True)
+    g.ax_heatmap.set_yticks([])
+    g.ax_heatmap.set_ylabel('')
+    g.ax_heatmap.set_xlabel('')
+    if save:
+        plt.savefig(fn)
+    return g
+
+
+def highlight_key(color_dir: dict,
+                  new_value: str = '#8a8787',
+                  key_to_highlight: list = ['Cardiac muscle lineages']
+                  ) -> dict:
+    """
+    Highlight one or more interested keys/celltypes when plotting,
+    the rest of keys/celltypes will be set to gray by default.
+    :param color_dir
+    :param new_value
+    :param key_to_highlight
+    :return dict
+    """
+    # assert key_to_highlight in color_dir.keys()
+    for k, v in color_dir.items():
+        if k not in key_to_highlight:
+            color_dir[k] = new_value
+    return color_dir
 
 
-def is_regulon_name(reg):
+def plot_legend(color_dir, marker='o', linestyle='', numpoints=1, ncol=3, loc='center', figsize=(10, 5),
+                fn='legend.png', **kwargs):
     """
-    Decide if a string is a regulon_list name
-    :param reg: the name of the regulon
+    Make separate legend file for heatmap
+    :param color_dir:
+    :param linestyle: legend icon style
+    :param marker: legend icon style
+    :param numpoints:
+    :param ncol: number of columns, legend layout
+    :param loc: location of the legend
+    :param figsize: (width, height)
+    :param fn:
+    :param kwargs:
     :return:
+
+    Example:
+        color_dir = {'celltype1': #000000}
+        plot_legend(color_dir)
     """
-    if '(+)' in reg or '(-)' in reg:
-        return True
+    fig = plt.figure(figsize=figsize)
+    markers = [plt.Line2D([0, 0], [0, 0], color=color, marker=marker, linestyle=linestyle, **kwargs)
+               for color in color_dir.values()]
+    plt.legend(markers, color_dir.keys(), numpoints=numpoints, ncol=ncol, loc=loc)
+    plt.box(False)
+    plt.xticks([])
+    plt.yticks([])
+    plt.tight_layout()
+    plt.savefig(fn)
+    plt.close()
 
 
-# Generate a heatmap
-def palplot(pal, names, colors=None, size=1):
+def get_top_regulons(data: anndata.AnnData, cluster_label: str, rss_celltype: pd.DataFrame, topn: int) -> list:
     """
+    get top n regulons for each cell type based on regulon specificity scores (rss)
+    :param data:
+    :param cluster_label:
+    :param rss_celltype:
+    :param topn:
+    :return: a list
+    """
+    # Select the top 5 regulon_list from each cell type
+    cats = sorted(list(set(data.obs[cluster_label])))
+    topreg = []
+    for i, c in enumerate(cats):
+        topreg.extend(
+            list(rss_celltype.T[c].sort_values(ascending=False)[:topn].index)
+        )
+    topreg = list(set(topreg))
+    return topreg
+
 
-    :param pal:
-    :param names:
-    :param colors:
-    :param size:
+def cal_zscore(auc_mtx: pd.DataFrame, save=False) -> pd.DataFrame:
+    """
+    calculate z-score for each gene among cells
+    :param auc_mtx:
+    :param save:
     :return:
     """
-    n = len(pal)
-    f, ax = plt.subplots(1, 1, figsize=(n * size, size))
-    ax.imshow(np.arange(n).reshape(1, n), cmap=mpl.colors.ListedColormap(list(pal)), interpolation="nearest",
-              aspect="auto")
-    ax.set_xticks(np.arange(n) - .5)
-    ax.set_yticks([-.5, .5])
-    ax.set_xticklabels([])
-    ax.set_yticklabels([])
-    colors = n * ['k'] if colors is None else colors
-    for idx, (name, color) in enumerate(zip(names, colors)):
-        ax.text(0.0 + idx, 0.0, name, color=color, horizontalalignment='center', verticalalignment='center')
-    return f
-
+    func = lambda x: (x - x.mean()) / x.std(ddof=0)
+    auc_zscore = auc_mtx.transform(func, axis=0)
+    if save:
+        auc_zscore.to_csv('auc_zscore.csv', index=False)
+    return auc_zscore
 
-def plot_legend(colormap, obs_list, legend_fn):
-    # plot legend
-    sns.set()
-    sns.set(font_scale=0.8)
-    palplot(colormap, obs_list, size=1)
-    plt.savefig(legend_fn, bbox_inches="tight")
-    plt.close()
 
+if __name__ == '__main__':
+    # total celltypes for Drosophilidae data
+    cluster_list = ['CNS', 'amnioserosa', 'carcass', 'epidermis', 'epidermis/CNS', 'fat body', 'fat body/trachea',
+                'foregut', 'foregut/garland cells', 'hemolymph', 'hindgut', 'hindgut/malpighian tubule', 'midgut',
+                'midgut/malpighian tubules', 'muscle', 'salivary gland', 'testis', 'trachea']
```

### Comparing `spagrn-1.0.4/spagrn/regulatory_network.py` & `spagrn-1.0.5/spagrn/regulatory_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         self._auc_mtx = None  # pd.DataFrame
         self._adjacencies = None  # pd.DataFrame
         self._regulon_dict = None  # dictionary
         self._rss = None  # pd.DataFrame
 
         # other settings
         self._params = {
-             'hotspot': {
+            'hotspot': {
                 'rank_threshold': 1500,
                 'prune_auc_threshold': 0.07,
                 'nes_threshold': 3.0,
                 'motif_similarity_fdr': 0.05,
                 'auc_threshold': 0.5,
                 'noweights': False,
             },
@@ -324,15 +324,15 @@
 
         Example:
             grn = InferenceRegulatoryNetwork(data)
             grn.add_params('hotspot', {'num_worker':12, 'auc_threshold': 0.001})
         """
         og_params = deepcopy(self._params)
         try:
-            for key, value in dic:
+            for key, value in dic.items():
                 self._params[method][key] = value
         except KeyError:
             logger.warning('KeyError, params did not change')  # TODO
             self._params = og_params
 
     def load_data_info(self, pos_label):
         """
@@ -420,15 +420,15 @@
         """
         data = InferRegulatoryNetwork.read_file(fn)
         if isinstance(data, anndata.AnnData):
             return data[data.obs[cluster_label].isin(target_clusters)]
         else:
             raise TypeError('data must be anndata.Anndata object')
 
-    @staticmethod
+    # @staticmethod
     # def load_stdata_by_cluster(data: StereoExpData,
     #                            meta: pd.DataFrame,
     #                            cluster_label: str,
     #                            target_clusters: list) -> scipy.sparse.csc_matrix:
     #     """
     #
     #     :param data:
@@ -606,14 +606,17 @@
         :param save: if save results onto disk
         :param jobs: Number of parallel jobs to run
         :param fn: output file name
         :return: A dataframe, local correlation Z-scores between genes (shape is genes x genes)
         """
         if os.path.isfile('local_correlations.csv'):
             local_correlations = pd.read_csv('local_correlations.csv', index_col=0)
+        elif os.path.isfile(fn):  # 2023-05-23: TODO: check what should be the index
+            local_correlations = pd.read_csv(fn)
+            return local_correlations
         else:
             hs = hotspot.Hotspot(data,
                                  layer_key=layer_key,
                                  model=model,
                                  latent_obsm_key=latent_obsm_key,
                                  umi_counts_obs_key=umi_counts_obs_key,
                                  **kwargs)
@@ -634,14 +637,16 @@
             common_tf_list = local_correlations.columns
 
         # reshape matrix
         local_correlations['TF'] = local_correlations.columns
         local_correlations = local_correlations.melt(id_vars=['TF'])
         local_correlations.columns = ['TF', 'target', 'importance']
         local_correlations = local_correlations[local_correlations.TF.isin(common_tf_list)]
+        # TODO: change variable name from local_correlations to adjs
+
         # remove if TF = target
         local_correlations = local_correlations[local_correlations.TF != local_correlations.target]
 
         if save:
             local_correlations.to_csv(fn, index=False)
         return local_correlations
 
@@ -798,19 +803,22 @@
                          regulons,
                          auc_threshold=auc_threshold,
                          num_workers=num_workers,
                          noweights=noweights,
                          normalize=normalize,
                          seed=seed,
                          **kwargs)
-        # check if there were regulons contain all zero auc values
-        if not auc_mtx.loc[:, auc_mtx.ne(0).any()].empty:
-            logger.warning('auc matrix contains all zero columns')
-        auc_mtx = auc_mtx.loc[:, ~auc_mtx.ne(0).any()]
-        
+
+        def remove_all_zero(auc_mtx):
+            # check if there were regulons contain all zero auc values
+            if not auc_mtx.loc[:, auc_mtx.ne(0).any()].empty:
+                logger.warning('auc matrix contains all zero columns')
+            auc_mtx = auc_mtx.loc[:, ~auc_mtx.ne(0).any()]
+            return auc_mtx
+
         self.auc_mtx = auc_mtx
 
         if save:
             auc_mtx.to_csv(fn)
         return auc_mtx
 
     # ------------------------------------------------------#
@@ -927,17 +935,17 @@
              sigm=15,
              prefix: str = 'project',
 
              layers='raw_counts',
              model='bernoulli',
              latent_obsm_key='spatial',
              umi_counts_obs_key=None,
-             cluster_label='annotation',
+             cluster_label='annotation',  # TODO: shouldn't set default value
 
-             noweights = None ,
+             noweights=None,
              normalize: bool = False):
         """
 
         :param databases:
         :param motif_anno_fn:
         :param tfs_fn:
         :param target_genes:
@@ -962,15 +970,15 @@
         df = self._data.to_df()
 
         if num_workers is None:
             num_workers = cpu_count()
 
         if target_genes is None:
             target_genes = self._gene_names
-        
+
         if noweights is None:
             noweights = self.params[method]["noweights"]
 
         # 1. load TF list
         if tfs_fn is None:
             tfs = 'all'
             # tfs = self._gene_names
@@ -1018,14 +1026,15 @@
                                       fn=f'{prefix}_motifs.csv',
                                       rank_threshold=self.params[method]["rank_threshold"],
                                       auc_threshold=self.params[method]["prune_auc_threshold"],
                                       nes_threshold=self.params[method]["nes_threshold"],
                                       motif_similarity_fdr=self.params[method]["motif_similarity_fdr"])
 
         self.regulon_dict = self.get_regulon_dict(regulons)
+        self.regulons_to_json(regulons, fn=f'{prefix}_regulons.json')
 
         # 5: Cellular enrichment (aka AUCell)
         auc_matrix = self.auc_activity_level(df,
                                              regulons,
                                              auc_threshold=self.params[method]["auc_threshold"],
                                              num_workers=num_workers,
                                              save=save,
@@ -1034,13 +1043,13 @@
                                              normalize=normalize,
                                              fn=f'{prefix}_auc.csv')
         logger.info('auc calculation DONE')
 
         self.cal_regulon_score(cluster_label=cluster_label, fn=f'{prefix}_regulon_specificity_scores.txt')
 
         # save results
-        if save:
-            logger.info('saving results...')
-            self.regulons_to_json(regulons, fn=f'{prefix}_regulons.json')
-            self.to_loom(df, auc_matrix, regulons, fn=f'{prefix}_output.loom')
+        # if save:
+            # logger.info('saving results...')
+            # self.regulons_to_json(regulons, fn=f'{prefix}_regulons.json')
+            # self.to_loom(df, auc_matrix, regulons, fn=f'{prefix}_output.loom')
             # self.to_cytoscape(regulons, adjacencies, 'Zfp354c')
-            logger.info('results saving DONE')
+            # logger.info('results saving DONE')
```

### Comparing `spagrn-1.0.4/spagrn/spa_logger.py` & `spagrn-1.0.5/spagrn/spa_logger.py`

 * *Files identical despite different names*

### Comparing `spagrn-1.0.4/spagrn/test.py` & `spagrn-1.0.5/spagrn/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """
 
 import os
 import sys
 import argparse
 from multiprocessing import cpu_count
 from regulatory_network import InferRegulatoryNetwork as irn
-from plot import PlotRegulatoryNetwork as prn
+import plot as prn
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='spaGRN tester')
     parser.add_argument("--data", '-i', type=str, help='experiment data file, in h5ad/loom format')
     parser.add_argument("--tf", '-t', type=str, help='TF list file')
     parser.add_argument("--database", '-d', type=str, help='ranked motifs database file, in feather format')
@@ -39,15 +39,14 @@
 
     # load data
     data = irn.read_file(fn)
     data = irn.preprocess(data)
 
     # create grn
     grn = irn(data)
-    grn_plot = prn(data)
 
     # run analysis
     grn.main(database_fn,
              motif_anno_fn,
              tfs_fn,
              num_workers=cpu_count(),
              cache=False,
```

### Comparing `spagrn-1.0.4/spagrn.egg-info/PKG-INFO` & `spagrn-1.0.5/spagrn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: spagrn
-Version: 1.0.4
+Version: 1.0.5
 Summary: A comprehensive tool to infer TF-centered, spatial gene regulatory networks for the spatially resolved transcriptomic data.
 Home-page: https://github.com/BGI-Qingdao/SpaGRN
 Author: Yao LI, Lidong GUO, Mengyang XU
 Author-email: liyao1@genomics.cn, guolidong@genomics.cn, xumengyang@genomics.cn
 License: GPL-3.0+
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.11
 License-File: LICENSE
-
-UNKNOWN
-
```

