# Comparing `tmp/PyComplexHeatmap-1.5.0.tar.gz` & `tmp/PyComplexHeatmap-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyComplexHeatmap-1.5.0.tar", last modified: Tue May 23 20:51:27 2023, max compression
+gzip compressed data, was "PyComplexHeatmap-1.5.1.tar", last modified: Fri Jun 16 19:01:38 2023, max compression
```

## Comparing `PyComplexHeatmap-1.5.0.tar` & `PyComplexHeatmap-1.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-05-23 20:51:27.917675 PyComplexHeatmap-1.5.0/
--rw-r--r--   0 wding      (503) staff       (20)     1067 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.5.0/LICENSE
--rw-r--r--   0 wding      (503) staff       (20)      105 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.5.0/MANIFEST.in
--rw-r--r--   0 wding      (503) staff       (20)    11704 2023-05-23 20:51:27.917290 PyComplexHeatmap-1.5.0/PKG-INFO
-drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-05-23 20:51:27.914965 PyComplexHeatmap-1.5.0/PyComplexHeatmap/
--rw-r--r--   0 wding      (503) staff       (20)      387 2023-05-23 20:49:55.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/__init__.py
--rw-r--r--   0 wding      (503) staff       (20)    66115 2023-05-16 22:49:47.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/annotations.py
--rw-r--r--   0 wding      (503) staff       (20)    75856 2023-05-23 20:30:33.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/clustermap.py
--rw-r--r--   0 wding      (503) staff       (20)     5430 2023-05-15 19:27:29.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/colors.py
--rw-r--r--   0 wding      (503) staff       (20)    21247 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/dotHeatmap.py
--rw-r--r--   0 wding      (503) staff       (20)     6766 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/example.py
--rw-r--r--   0 wding      (503) staff       (20)    17848 2023-05-17 00:12:40.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/oncoPrint.py
--rw-r--r--   0 wding      (503) staff       (20)     6753 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/tools.py
--rw-r--r--   0 wding      (503) staff       (20)    28823 2023-05-23 20:47:26.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap/utils.py
-drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-05-23 20:51:27.916757 PyComplexHeatmap-1.5.0/PyComplexHeatmap.egg-info/
--rw-r--r--   0 wding      (503) staff       (20)    11704 2023-05-23 20:51:27.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap.egg-info/PKG-INFO
--rw-r--r--   0 wding      (503) staff       (20)      473 2023-05-23 20:51:27.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap.egg-info/SOURCES.txt
--rw-r--r--   0 wding      (503) staff       (20)        1 2023-05-23 20:51:27.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap.egg-info/dependency_links.txt
--rw-r--r--   0 wding      (503) staff       (20)       17 2023-05-23 20:51:27.000000 PyComplexHeatmap-1.5.0/PyComplexHeatmap.egg-info/top_level.txt
--rw-r--r--   0 wding      (503) staff       (20)    11095 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.5.0/README.md
--rw-r--r--   0 wding      (503) staff       (20)      672 2023-05-23 20:50:06.000000 PyComplexHeatmap-1.5.0/pyproject.toml
--rw-r--r--   0 wding      (503) staff       (20)       38 2023-05-23 20:51:27.917773 PyComplexHeatmap-1.5.0/setup.cfg
--rw-r--r--   0 wding      (503) staff       (20)     1044 2023-05-23 20:50:15.000000 PyComplexHeatmap-1.5.0/setup.py
+drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-06-16 19:01:38.429423 PyComplexHeatmap-1.5.1/
+-rw-r--r--   0 wding      (503) staff       (20)     1067 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.5.1/LICENSE
+-rw-r--r--   0 wding      (503) staff       (20)      105 2023-05-16 21:30:04.000000 PyComplexHeatmap-1.5.1/MANIFEST.in
+-rw-r--r--   0 wding      (503) staff       (20)    11894 2023-06-16 19:01:38.428834 PyComplexHeatmap-1.5.1/PKG-INFO
+drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-06-16 19:01:38.425075 PyComplexHeatmap-1.5.1/PyComplexHeatmap/
+-rw-r--r--   0 wding      (503) staff       (20)      387 2023-06-16 18:59:50.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/__init__.py
+-rw-r--r--   0 wding      (503) staff       (20)    66619 2023-06-16 18:42:57.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/annotations.py
+-rw-r--r--   0 wding      (503) staff       (20)    75826 2023-06-16 18:44:04.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/clustermap.py
+-rw-r--r--   0 wding      (503) staff       (20)     5430 2023-05-15 19:27:29.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/colors.py
+-rw-r--r--   0 wding      (503) staff       (20)    21257 2023-06-09 16:20:57.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/dotHeatmap.py
+-rw-r--r--   0 wding      (503) staff       (20)     6766 2023-05-08 23:39:01.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/example.py
+-rw-r--r--   0 wding      (503) staff       (20)    17872 2023-06-09 16:23:11.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/oncoPrint.py
+-rw-r--r--   0 wding      (503) staff       (20)     6788 2023-06-09 16:21:38.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/tools.py
+-rw-r--r--   0 wding      (503) staff       (20)    28836 2023-06-16 17:06:16.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap/utils.py
+drwxr-xr-x   0 wding      (503) staff       (20)        0 2023-06-16 19:01:38.428084 PyComplexHeatmap-1.5.1/PyComplexHeatmap.egg-info/
+-rw-r--r--   0 wding      (503) staff       (20)    11894 2023-06-16 19:01:38.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap.egg-info/PKG-INFO
+-rw-r--r--   0 wding      (503) staff       (20)      473 2023-06-16 19:01:38.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 wding      (503) staff       (20)        1 2023-06-16 19:01:38.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 wding      (503) staff       (20)       17 2023-06-16 19:01:38.000000 PyComplexHeatmap-1.5.1/PyComplexHeatmap.egg-info/top_level.txt
+-rw-r--r--   0 wding      (503) staff       (20)    11285 2023-06-09 04:09:45.000000 PyComplexHeatmap-1.5.1/README.md
+-rw-r--r--   0 wding      (503) staff       (20)      686 2023-06-16 18:59:11.000000 PyComplexHeatmap-1.5.1/pyproject.toml
+-rw-r--r--   0 wding      (503) staff       (20)       38 2023-06-16 19:01:38.429647 PyComplexHeatmap-1.5.1/setup.cfg
+-rw-r--r--   0 wding      (503) staff       (20)     1044 2023-06-16 18:59:26.000000 PyComplexHeatmap-1.5.1/setup.py
```

### Comparing `PyComplexHeatmap-1.5.0/LICENSE` & `PyComplexHeatmap-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.5.0/PKG-INFO` & `PyComplexHeatmap-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.5.0
+Version: 1.5.1
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
 Classifier: Programming Language :: Python :: 3
@@ -33,19 +33,23 @@
 
 ## Dependencies:
 ----------------------
 - matplotlib>=3.4.3
 - numpy
 - pandas
 - scipy
+- fastcluster
 ```
 pip install --ignore-install matplotlib==3.5.1 numpy==1.20.3 pandas==1.4.1
 pip install seaborn #only needed when call functions in tools.py
 ```
 
+## Citation
+Ding, W., Goldberg, D. and Zhou, W. (2023), PyComplexHeatmap: A Python package to visualize multimodal genomics data. iMeta e115. https://doi.org/10.1002/imt2.115
+
 ## **Installation**
 ----------------------
 1. **Install using pip**:
 ```shell
 pip install PyComplexHeatmap
 
 #upgrade from older version
```

### Comparing `PyComplexHeatmap-1.5.0/PyComplexHeatmap/annotations.py` & `PyComplexHeatmap-1.5.1/PyComplexHeatmap/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,32 +149,32 @@
                 self.cmap = 'jet'
             else:
                 raise TypeError("Can not assign cmap for column %s, please specify cmap" % col)
         elif type(cmap) == str:
             self.cmap = cmap
         else:
             raise TypeError("Unknow data type for cmap!")
-        if plt.get_cmap(self.cmap).N == 256:  # then heatmap will automatically calculate vmin and vmax
+        if plt.colormaps.get(self.cmap).N == 256:  # then heatmap will automatically calculate vmin and vmax
             try:
                 self.plot_kws.setdefault('vmax', np.nanmax(self.df.values))
                 self.plot_kws.setdefault('vmin', np.nanmin(self.df.values))
             except:
                 pass
 
     def _calculate_colors(self):  # add self.color_dict (each col is a dict)
         self.color_dict = {}
         col = self.df.columns.tolist()[0]
-        if plt.get_cmap(self.cmap).N < 256 or self.df.dtypes[col] == object:
+        if plt.colormaps.get(self.cmap).N < 256 or self.df.dtypes[col] == object:
             cc_list = self.df[col].value_counts().index.tolist()  # sorted by value counts
             self.df[col] = self.df[col].map({v: cc_list.index(v) for v in cc_list})
             for v in cc_list:
-                color = plt.get_cmap(self.cmap)(cc_list.index(v))
+                color = plt.colormaps.get(self.cmap)(cc_list.index(v))
                 self.color_dict[v] = color  # matplotlib.colors.to_hex(color)
         else:  # float
-            self.color_dict = {v: plt.get_cmap(self.cmap)(v) for v in self.df[col].values}
+            self.color_dict = {v: plt.colormaps.get(self.cmap)(v) for v in self.df[col].values}
         self.colors = None
 
     def _check_colors(self, colors):
         if isinstance(colors, str):
             colors = {label: colors for label in self.df.iloc[:, 0].unique()}
         if isinstance(colors, list):
             assert len(colors) == self.df.iloc[:, 0].nunique()
@@ -188,15 +188,15 @@
 
     def _calculate_cmap(self):
         self.color_dict = self.colors
         col = self.df.columns.tolist()[0]
         cc_list = list(self.color_dict.keys())  # column values
         self.df[col] = self.df[col].map({v: cc_list.index(v) for v in cc_list})
         self.cmap = matplotlib.colors.ListedColormap([self.color_dict[k] for k in cc_list])
-        self.plot_kws.setdefault('vmax', plt.get_cmap(self.cmap).N)
+        self.plot_kws.setdefault('vmax', plt.colormaps.get(self.cmap).N)
         self.plot_kws.setdefault('vmin', 0)
 
     def _type_specific_params(self):
         pass
 
     def reorder(self, idx):  # Before plotting, df needs to be reordered according to the new clustered order.
         """
@@ -252,37 +252,41 @@
         self.text_kws.setdefault('zorder', 16)
         self.text_kws.setdefault('ha', 'center')
         self.text_kws.setdefault('va', 'center')
 
     def _calculate_colors(self):  # add self.color_dict (each col is a dict)
         self.color_dict = {}
         col = self.df.columns.tolist()[0]
-        if plt.get_cmap(self.cmap).N < 256:
+        if plt.colormaps.get(self.cmap).N < 256:
             cc_list = self.df[col].value_counts().index.tolist()  # sorted by value counts
             for v in cc_list:
-                color = plt.get_cmap(self.cmap)(cc_list.index(v))
+                color = plt.colormaps.get(self.cmap)(cc_list.index(v))
                 self.color_dict[v] = color  # matplotlib.colors.to_hex(color)
         else:  # float
             cc_list = None
-            self.color_dict = {v: plt.get_cmap(self.cmap)(v) for v in self.df[col].values}
+            self.color_dict = {v: plt.colormaps.get(self.cmap)(v) for v in self.df[col].values}
         self.cc_list = cc_list
         self.colors = None
 
     def _calculate_cmap(self):
         self.color_dict = self.colors
         col = self.df.columns.tolist()[0]
         cc_list = list(self.color_dict.keys())  # column values
         self.cc_list = cc_list
         self.cmap = matplotlib.colors.ListedColormap([self.color_dict[k] for k in cc_list])
-        self.plot_kws.setdefault('vmax', plt.get_cmap(self.cmap).N)
-        self.plot_kws.setdefault('vmin', 0)
 
     def plot(self, ax=None, axis=1, subplot_spec=None, label_kws={},
              ticklabels_kws={}):  # add self.gs,self.fig,self.ax,self.axes
-        self.plot_kws.setdefault('vmax', plt.get_cmap(self.cmap).N)
+        if hasattr(self.cmap,'N'):
+            vmax=self.cmap.N
+        elif type(self.cmap)==str:
+            vmax=plt.colormaps.get(self.cmap).N
+        else:
+            vmax=len(self.color_dict)
+        self.plot_kws.setdefault('vmax',vmax)  # plt.colormaps.get(self.cmap).N
         self.plot_kws.setdefault('vmin', 0)
         if self.cc_list:
             mat = self.plot_data.iloc[:, 0].map({v: self.cc_list.index(v) for v in self.cc_list}).values
         else:
             mat = self.plot_data.values
         matrix = mat.reshape(1, -1) if axis == 1 else mat.reshape(-1, 1)
         # print(matrix)
@@ -408,21 +412,21 @@
         # self.plot_kws.setdefault('transform_rotates_text', False)
         self.plot_kws.setdefault('arrowprops', arrowprops)
         self.plot_kws.setdefault('rotation_mode', 'anchor')
 
     def _calculate_colors(self):  # add self.color_dict (each col is a dict)
         self.color_dict = {}
         col = self.df.columns.tolist()[0]
-        if plt.get_cmap(self.cmap).N < 256 or self.df.dtypes[col] == object:
+        if plt.colormaps.get(self.cmap).N < 256 or self.df.dtypes[col] == object:
             cc_list = self.df[col].value_counts().index.tolist()  # sorted by value counts
             for v in cc_list:
-                color = plt.get_cmap(self.cmap)(cc_list.index(v))
+                color = plt.colormaps.get(self.cmap)(cc_list.index(v))
                 self.color_dict[v] = color  # matplotlib.colors.to_hex(color)
         else:  # float
-            self.color_dict = {v: plt.get_cmap(self.cmap)(v) for v in self.df[col].values}
+            self.color_dict = {v: plt.colormaps.get(self.cmap)(v) for v in self.df[col].values}
         self.colors = None
 
     def _calculate_cmap(self):
         self.color_dict = self.colors
         col = self.df.columns.tolist()[0]
         cc_list = list(self.color_dict.keys())  # column values
         self.cmap = matplotlib.colors.ListedColormap([self.color_dict[k] for k in cc_list])
@@ -590,15 +594,15 @@
         gap = self.df.max().max() - self.df.min().min()
         self.ylim = [self.df.min().min() - 0.02 * gap, self.df.max().max() + 0.02 * gap]
 
     def plot(self, ax=None, axis=1, subplot_spec=None, label_kws={},
              ticklabels_kws={}):  # add self.gs,self.fig,self.ax,self.axes
         fig = ax.figure
         if self.colors is None:  # calculate colors based on cmap
-            colors = [plt.get_cmap(self.cmap)(self.plot_data.loc[sampleID].mean()) for sampleID in
+            colors = [plt.colormaps.get(self.cmap)(self.plot_data.loc[sampleID].mean()) for sampleID in
                       self.plot_data.index.values]
         else:
             colors = [self.colors] * self.plot_data.shape[0]  # self.colors is a string
         # print(self.plot_kws)
         plot_kws = self.plot_kws.copy()
         edgecolor = plot_kws.pop('edgecolor')
         mlinecolor = plot_kws.pop('medianlinecolor')
@@ -655,31 +659,33 @@
             if self.ncols == 1:
                 self.cmap = 'jet'
             else:
                 self.cmap = 'Set1'
         # print(cmap,self.cmap)
         else:
             self.cmap = cmap
-        if self.ncols >= 2 and plt.get_cmap(self.cmap).N >= 256:
+        if self.ncols >= 2 and plt.colormaps.get(self.cmap).N >= 256:
             raise TypeError("cmap for stacked barplot should not be continuous, you should try: Set1, Dark2 and so on.")
 
     def _calculate_colors(self):  # add self.color_dict (each col is a dict)
         col_list = self.df.columns.tolist()
         self.color_dict = {}
         if len(col_list) >= 2:  # more than two columns, colored by columns names
-            self.colors = [plt.get_cmap(self.cmap)(col_list.index(v)) for v in self.df.columns]
+            self.colors = [plt.colormaps.get(self.cmap)(col_list.index(v)) for v in self.df.columns]
             for v, color in zip(col_list, self.colors):
                 self.color_dict[v] = color
         else:  # only one column, colored by cols[0] values (float)
             # vmax, vmin = np.nanmax(self.df[col_list[0]].values), np.nanmin(self.df[col_list[0]].values)
             # delta = vmax - vmin
             # values = self.df[col_list[0]].fillna(np.nan).unique()
-            self.cmap,normalize=define_cmap(self.df[col_list[0]].fillna(np.nan).values, vmin=None, vmax=None, cmap=self.cmap, center=None, robust=False,
+            self.cmap,normalize=define_cmap(self.df[col_list[0]].fillna(np.nan).values,
+                                            vmin=None, vmax=None, cmap=self.cmap,
+                                            center=None, robust=False,
                           na_col='white')
-            # self.colors = {v: matplotlib.colors.rgb2hex(plt.get_cmap(self.cmap)((v - vmin) / delta)) for v in values}
+            # self.colors = {v: matplotlib.colors.rgb2hex(plt.colormaps.get(self.cmap)((v - vmin) / delta)) for v in values}
             self.colors = lambda v:matplotlib.colors.rgb2hex(self.cmap(normalize(v))) #a function
             self.color_dict = None
 
     def _check_colors(self, colors):
         if not isinstance(colors, (list, str)):
             raise TypeError("colors must be list of string for barplot if provided !")
         if type(colors) == str:
@@ -720,15 +726,15 @@
         if grid:
             ax.grid(linestyle='--', zorder=-10)
         # bar_ct = ax.bar(x=list(range(1, self.nrows + 1,1)),
         #                 height=self.plot_data.values,**self.plot_kws)
         if type(self.colors) == list:
             colors = self.colors
         else: #dict
-            #bad_value_color = matplotlib.colors.rgb2hex(plt.get_cmap(self.cmap).get_bad())
+            #bad_value_color = matplotlib.colors.rgb2hex(plt.colormaps.get(self.cmap).get_bad())
             # colors = [[self.colors.get(v, bad_value_color) for v in self.plot_data.iloc[:, 0].values]]
             colors = [[self.colors(v) for v in self.plot_data.iloc[:, 0].values]]
         base_coordinates = [0] * self.plot_data.shape[0]
         for col, color in zip(self.plot_data.columns, colors):
             if axis == 1:
                 ax.set_xticks(ticks=np.arange(0.5, self.nrows, 1))
                 ax.bar(x=np.arange(0.5, self.nrows, 1), height=self.plot_data[col].values,
@@ -778,15 +784,15 @@
     def _check_cmap(self, cmap):
         self.cmap = 'jet'
         if cmap == 'auto':
             pass
         elif type(cmap) == str:
             self.cmap = cmap
         else:
-            raise TypeError("cmap for boxplot should be a string")
+            raise TypeError("cmap for scatterplot should be a string")
 
     def _calculate_colors(self):  # add self.color_dict (each col is a dict)
         self.colors = None
 
     def _check_colors(self, colors):
         if not isinstance(colors, str):
             raise TypeError("colors must be string for scatterplot, if more colors are neded, please try cmap!")
@@ -1202,27 +1208,31 @@
         if self.verbose >= 1:
             print("Collecting annotation legends..")
         self.legend_list = []  # handles(dict) / cmap, title, kws
         for annotation in self.annotations:
             if not annotation.legend:
                 continue
             legend_kws = annotation.legend_kws.copy()
-            if annotation.cmap is None or plt.get_cmap(annotation.cmap).N < 256:
+            # print(annotation.cmap,annotation)
+            if (annotation.cmap is None) or \
+                (hasattr(annotation.cmap,'N') and annotation.cmap.N < 256) or \
+                (type(annotation.cmap) ==str and plt.colormaps.get(annotation.cmap).N < 256):
                 color_dict = annotation.color_dict
                 if color_dict is None:
                     continue
                 self.legend_list.append(
                     [annotation.color_dict, annotation.label, legend_kws, len(annotation.color_dict),'color_dict'])
             else:
                 if annotation.df.shape[1] == 1:
                     array = annotation.df.iloc[:, 0].values
                 else:
                     array = annotation.df.values
                 vmax = np.nanmax(array)
                 vmin = np.nanmin(array)
+                # print(vmax,vmin,annotation)
                 legend_kws.setdefault('vmin', round(vmin, 2))
                 legend_kws.setdefault('vmax', round(vmax, 2))
                 self.legend_list.append([annotation.cmap, annotation.label, legend_kws, 4,'cmap'])
         if len(self.legend_list) > 1:
             self.legend_list = sorted(self.legend_list, key=lambda x: x[3])
         if self.label_side == 'right':
             self.label_max_width = max([ann.get_max_label_width() for ann in self.annotations])
```

### Comparing `PyComplexHeatmap-1.5.0/PyComplexHeatmap/clustermap.py` & `PyComplexHeatmap-1.5.1/PyComplexHeatmap/clustermap.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,27 +131,27 @@
                 vmax = np.nanmax(calc_data)
         self.vmin, self.vmax = vmin, vmax
 
         # Choose default colormaps if not provided
         if cmap is None:
             if center is None:
                 try:
-                    self.cmap = matplotlib.cm.get_cmap('turbo').copy()
+                    self.cmap = plt.colormaps.get('turbo').copy()
                 except:
-                    self.cmap = matplotlib.cm.get_cmap('turbo')
+                    self.cmap = plt.colormaps.get('turbo')
             else:
                 try:
-                    self.cmap = matplotlib.cm.get_cmap('exp1').copy()
+                    self.cmap = plt.colormaps.get('exp1').copy()
                 except:
-                    self.cmap = matplotlib.cm.get_cmap('exp1')
+                    self.cmap = plt.colormaps.get('exp1')
         elif isinstance(cmap, str):
             try:
-                self.cmap = matplotlib.cm.get_cmap(cmap).copy()
+                self.cmap = plt.colormaps.get(cmap).copy()
             except:
-                self.cmap = matplotlib.cm.get_cmap(cmap)
+                self.cmap = plt.colormaps.get(cmap)
         elif isinstance(cmap, list):
             self.cmap = matplotlib.colors.ListedColormap(cmap)
         else:
             self.cmap = cmap
 
         self.cmap.set_bad(color=self.na_col)  # set the color for NaN values
         # Recenter a divergent colormap
@@ -447,17 +447,17 @@
             vmax = np.nanpercentile(calc_data, 98)
         else:
             vmax = np.nanmax(calc_data)
 
     # Choose default colormaps if not provided
     if isinstance(cmap, str):
         try:
-            cmap = matplotlib.cm.get_cmap(cmap).copy()
+            cmap = plt.colormaps.get(cmap).copy()
         except:
-            cmap = matplotlib.cm.get_cmap(cmap)
+            cmap = plt.colormaps.get(cmap)
 
     cmap.set_bad(color=na_col)  # set the color for NaN values
     # Recenter a divergent colormap
     if center is not None:
         # bad = cmap(np.ma.masked_invalid([np.nan]))[0]  # set the first color as the na_color
         under = cmap(-np.inf)
         over = cmap(np.inf)
@@ -1235,15 +1235,15 @@
                 ax1.set_axis_off()
                 self.ax_row_dendrogram_axes.append(ax1)
 
             try:
                 if rcmap is None:
                     colors = ['black'] * len(self.dendrogram_rows)
                 else:
-                    colors = [plt.get_cmap(rcmap)(i) for i in range(len(self.dendrogram_rows))]
+                    colors = [plt.colormaps.get(rcmap)(i) for i in range(len(self.dendrogram_rows))]
                 for ax_row_dendrogram, dendrogram_row, color in zip(self.ax_row_dendrogram_axes, self.dendrogram_rows,
                                                                     colors):
                     if dendrogram_row is None:
                         continue
                     tree_kws['colors'] = [color] * len(dendrogram_row.dendrogram['ivl'])
                     dendrogram_row.plot(ax=ax_row_dendrogram, tree_kws=tree_kws)
             except:
@@ -1264,15 +1264,15 @@
                 ax1.set_axis_off()
                 self.ax_col_dendrogram_axes.append(ax1)
 
             try:
                 if ccmap is None:
                     colors = ['black'] * len(self.dendrogram_cols)
                 else:
-                    colors = [plt.get_cmap(ccmap)(i) for i in range(len(self.dendrogram_cols))]
+                    colors = [plt.colormaps.get(ccmap)(i) for i in range(len(self.dendrogram_cols))]
                 for ax_col_dendrogram, dendrogram_col, color in zip(self.ax_col_dendrogram_axes, self.dendrogram_cols,
                                                                     colors):
                     if dendrogram_col is None:
                         continue
                     tree_kws['colors'] = [color] * len(dendrogram_col.dendrogram['ivl'])
                     dendrogram_col.plot(ax=ax_col_dendrogram, tree_kws=tree_kws)
             except:
```

### Comparing `PyComplexHeatmap-1.5.0/PyComplexHeatmap/colors.py` & `PyComplexHeatmap-1.5.1/PyComplexHeatmap/colors.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.5.0/PyComplexHeatmap/dotHeatmap.py` & `PyComplexHeatmap-1.5.1/PyComplexHeatmap/dotHeatmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         kwargs.setdefault('cmap', cmap)
         c_ready = True
     elif not hue is None and isinstance(cmap,str):
         color_dict = {} #keys are categorical values from hue, values are colors.
         if colors is None:  #using cmap
             col_list = df['Hue'].value_counts().index.tolist()
             for c in col_list:
-                color_dict[c] = matplotlib.colors.to_hex(plt.get_cmap(cmap)(col_list.index(c)))
+                color_dict[c] = matplotlib.colors.to_hex(plt.colormaps.get(cmap)(col_list.index(c)))
         elif type(colors) == dict:
             color_dict = colors
         elif type(colors) == str:
             col_list = df['Hue'].value_counts().index.tolist()
             for c in col_list:
                 color_dict[c] = colors
         else:
@@ -400,15 +400,15 @@
                     self.label_max_width = annotation.label_max_width
         if self.legend:
             if isinstance(self.cmap,str) and not self.hue is None and self.c is None:  #
                 color_dict = {}
                 col_list = self.kwargs['hue'].unstack().value_counts().index.tolist()
                 # print(col_list,self.kwargs['hue'])
                 for c in col_list:
-                    color_dict[c] = matplotlib.colors.to_hex(plt.get_cmap(self.cmap)(col_list.index(c)))
+                    color_dict[c] = matplotlib.colors.to_hex(plt.colormaps.get(self.cmap)(col_list.index(c)))
                 self.legend_list.append([color_dict, self.hue, self.color_legend_kws, len(color_dict), 'color_dict'])
             cmap=self.cmap
             c=self.kwargs.get('c',None)
             cmap_legend_kws=self.cmap_legend_kws.copy()
             cmap_legend_kws['vmax'] = self.v_vmax
             cmap_legend_kws['vmin'] = self.v_vmin
             if not cmap is None and type(cmap) == str and not c is None and type(c)!=str:
```

### Comparing `PyComplexHeatmap-1.5.0/PyComplexHeatmap/example.py` & `PyComplexHeatmap-1.5.1/PyComplexHeatmap/example.py`

 * *Files identical despite different names*

### Comparing `PyComplexHeatmap-1.5.0/PyComplexHeatmap/oncoPrint.py` & `PyComplexHeatmap-1.5.1/PyComplexHeatmap/oncoPrint.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     """
     if ax is None:
         ax = plt.gca()
     nrows, ncols = data.shape
     if nvar is None:
         nvar=data.iloc[:,0].apply(lambda x:len(x)).max()
     if colors is None:
-        colors=[plt.get_cmap(cmap)(i) for i in range(nvar)]
+        colors=[plt.colormaps.get(cmap)(i) for i in range(nvar)]
     plot_kws.setdefault('width',0.7)
     plot_kws.setdefault('align', 'center')
     rowticklabels=_index_to_ticklabels(data.index)
     colticklabels=_index_to_ticklabels(data.columns)
     ax.set_ylim(0, nrows)
     y_locater = list(np.arange(0.5, nrows, 1))
     ax.yaxis.set_major_locator(plt.FixedLocator(y_locater))
@@ -134,15 +134,15 @@
     bgcolor: str
         background color, default is whitesmoke (or lightgray)
     color_legend_kws: dict
         legend_kws passed to plot_color_dict_legend
     cmap_legend_kws: dict
         legend_kws passed to plot_cmap_legend
     kwargs :dict
-        Other kwargs passed to ClusterMapPlotter.
+        Other kwargs passed to ClusterMapPlotter and oncoprint.
 
     Returns
     -------
     oncoPrintPlotter.
     """
 
     def __init__(self, data=None, x=None, y=None, values=None, cmap='Set1',colors=None,
@@ -175,15 +175,15 @@
         if self.remove_empty_cols:
             data2d=data2d.loc[:,df_sum.sum(axis=0)>0]
         row_vc = data2d.apply(lambda x: x.apply(np.array).sum(), axis=1)
         self.row_vc = pd.DataFrame(row_vc.tolist(), index=row_vc.index.tolist(), columns=self.values)
         self.col_vc = data2d.apply(lambda x: x.apply(np.array).sum(), axis=0).T
         self.col_vc.columns=self.values
         if self.colors is None:
-            self.colors = [plt.get_cmap(self.cmap)(i) for i in range(len(self.values))]
+            self.colors = [plt.colormaps.get(self.cmap)(i) for i in range(len(self.values))]
         self.color_dict = {}
         for label, color in zip(self.values, self.colors):
             self.color_dict[label] = color
         return data2d
 
     def _reorder_rows(self):
         if self.verbose >= 1:
```

### Comparing `PyComplexHeatmap-1.5.0/PyComplexHeatmap/tools.py` & `PyComplexHeatmap-1.5.1/PyComplexHeatmap/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,31 +79,34 @@
 
     Returns
     -------
 
     """
     if not hue is None:
         hue_order=df[hue].unique().tolist() if hue_order is None else hue_order
-        color_dict={h:plt.get_cmap(cmap)(hue_order.index(h)) for h in hue_order}
+        color_dict={h:plt.colormaps.get(cmap)(hue_order.index(h)) for h in hue_order}
     else:
         color_dict=None
         hue_order=None
     N=list(range(1,df.shape[0]+1))
     s_min = np.nanmin(df[size].values)
     delta_s = np.nanmax(df[size].values) - s_min
     fig, ax = plt.subplots(figsize=figsize)
     w, h = ax.get_window_extent().width / ax.figure.dpi, ax.get_window_extent().height / ax.figure.dpi
     r = min(w * 72 / len(df.shape[1]), h * 72 / len(df.shape[0]))
     if not hue_order is None:
         for c in hue_order:
-            idx=np.where(df[hue].values==c)[0]
-            s=df.iloc[idx][size].apply(lambda x:(x-s_min) / delta_s) * (r**2) if type(size)==str else size
-            color1=color_dict[c] if not color_dict is None else color
-            ax.scatter(x=df.iloc[idx][x].tolist(),y=[N[i] for i in idx],
-                       s=s,color=color1,label=c)
+          idx = np.where(df[hue].values == c)[0]
+          if type(size) == str:
+              s = (df.iloc[idx][size] - s_min) / delta_s * r**2
+          else:
+              s = size
+          color1 = color_dict[c] if not color_dict is None else color
+          ax.scatter(x=df.iloc[idx][x].tolist(), y=[N[i] for i in idx],
+                     s=s, color=color1, label=c)
     else:
         s = df[size].apply(lambda x:(x-s_min) / delta_s) * (r**2) if type(size) == str else size
         ax.scatter(x=df[x].tolist(), y=N,
                    s=s, color=color, label=None)
 
     ax.set_ylim([0,len(N)+0.8])
     ax.set_xlabel(x)
@@ -190,8 +193,8 @@
                     textcoords='offset points')  # connectionstyle='arc3,rad=0.5',arrowprops=dict(arrowstyle='-',lw=0.5,color='black')
     for i, (x0, y0,t) in data.loc[data[hue] == hue_order[2],
                           [x, y,label]].sort_values(y,ascending=False).head(topn).iterrows():
         # print(t,x0,y0)
         ax.annotate(text=t, xy=(x0, y0), xytext=(0.1, 3), annotation_clip=False,
                     color=colors[2], textcoords='offset points')  # arrowprops=dict(arrowstyle='-',lw=0.5,color='black')
     plt.tight_layout()
-    plt.savefig(outname)
+    plt.savefig(outname)
```

### Comparing `PyComplexHeatmap-1.5.0/PyComplexHeatmap/utils.py` & `PyComplexHeatmap-1.5.1/PyComplexHeatmap/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 import matplotlib.lines as mlines
 import matplotlib.patches as mpatches
 mm2inch=1/25.4
 # =============================================================================
 def set_default_style():
     from matplotlib import rcParams
     D={
-        'font.family':['sans serif'], #'serif',
+        # 'font.family':['sans serif'], #'serif',
         # 'mathtext.fontset':'dejavuserif',
-        'font.sans-serif':['Arial'],
+        # 'font.sans-serif':['Arial'],
         'pdf.fonttype':42,
 
         # Remove legend frame
         'legend.frameon': True,
         'legend.fontsize': 10,
 
         # Savefig
@@ -594,16 +594,16 @@
         ax.set_axis_off()
         left=ax.get_position().x0+ax.yaxis.labelpad*2/ax.figure.get_window_extent().width if delta_x is None else ax.get_position().x0+delta_x
     else:
         #labelpad: Spacing in points, pad is the fraction relative to x1.
         pad = (space+ax.yaxis.labelpad*1.2*ax.figure.dpi / 72) / ax.figure.get_window_extent().width if delta_x is None else delta_x #labelpad unit is points
         left=ax.get_position().x1 + pad
     if legend_width is None:
-        legend_width=cal_legend_width(legend_list) + 2.5 #base width for color rectangle is set to 2 mm
-    # print("Estimated legend width: ",legend_width)
+        legend_width=cal_legend_width(legend_list) + 2.5 #base width for color rectangle is set to 2.5 mm
+        print(f"Estimated legend width: {legend_width} mm")
     legend_width=legend_width*mm2inch*ax.figure.dpi / ax.figure.get_window_extent().width #mm to px to fraction
     cmap_width = cmap_width * mm2inch * ax.figure.dpi / ax.figure.get_window_extent().width  # mm to px to fraction
     if legend_side=='right':
         ax_legend=ax.figure.add_axes([left,ax.get_position().y0,legend_width,ax.get_position().height]) #left, bottom, width, height
     legend_axes=[ax_legend]
     cbars=[]
     leg_pos = ax_legend.get_position() #left bototm: x0,y0; top right: x1,y1
```

### Comparing `PyComplexHeatmap-1.5.0/PyComplexHeatmap.egg-info/PKG-INFO` & `PyComplexHeatmap-1.5.1/PyComplexHeatmap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.5.0
+Version: 1.5.1
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 Project-URL: Homepage, https://github.com/DingWB/PyComplexHeatmap
 Project-URL: Bug Tracker, https://github.com/DingWB/PyComplexHeatmap/issues
 Classifier: Programming Language :: Python :: 3
@@ -33,19 +33,23 @@
 
 ## Dependencies:
 ----------------------
 - matplotlib>=3.4.3
 - numpy
 - pandas
 - scipy
+- fastcluster
 ```
 pip install --ignore-install matplotlib==3.5.1 numpy==1.20.3 pandas==1.4.1
 pip install seaborn #only needed when call functions in tools.py
 ```
 
+## Citation
+Ding, W., Goldberg, D. and Zhou, W. (2023), PyComplexHeatmap: A Python package to visualize multimodal genomics data. iMeta e115. https://doi.org/10.1002/imt2.115
+
 ## **Installation**
 ----------------------
 1. **Install using pip**:
 ```shell
 pip install PyComplexHeatmap
 
 #upgrade from older version
```

### Comparing `PyComplexHeatmap-1.5.0/README.md` & `PyComplexHeatmap-1.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,23 @@
 
 ## Dependencies:
 ----------------------
 - matplotlib>=3.4.3
 - numpy
 - pandas
 - scipy
+- fastcluster
 ```
 pip install --ignore-install matplotlib==3.5.1 numpy==1.20.3 pandas==1.4.1
 pip install seaborn #only needed when call functions in tools.py
 ```
 
+## Citation
+Ding, W., Goldberg, D. and Zhou, W. (2023), PyComplexHeatmap: A Python package to visualize multimodal genomics data. iMeta e115. https://doi.org/10.1002/imt2.115
+
 ## **Installation**
 ----------------------
 1. **Install using pip**:
 ```shell
 pip install PyComplexHeatmap
 
 #upgrade from older version
```

### Comparing `PyComplexHeatmap-1.5.0/pyproject.toml` & `PyComplexHeatmap-1.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0","matplotlib>=3.5.1","numpy>=1.20.3","pandas>=1.4.1", "scipy"]
+requires = ["setuptools>=61.0","matplotlib>=3.5.1","numpy>=1.20.3","pandas>=1.4.1", "scipy","fastcluster"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyComplexHeatmap"
-version = "1.5.0"
+version = "1.5.1"
 authors = [
   { name="Wubin Ding", email="ding.wu.bin.gm@gmail.com" },
 ]
 description = "A python package to plot complex heatmap"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `PyComplexHeatmap-1.5.0/setup.py` & `PyComplexHeatmap-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 # print(long_description)
 
 #release new version
 setup(
    name='PyComplexHeatmap',
-   version='1.5.0',
+   version='1.5.1',
    description='A Python package to plot complex heatmap',
    # long_description="#PyComplexHeatmap\n##Documentation:https://dingwb.github.io/PyComplexHeatmap/build/html/index.html",
    # long_description_content_type='text/markdown',
    author='Wubin Ding',
    author_email='ding.wu.bin.gm@gmail.com',
    url="https://github.com/DingWB/PyComplexHeatmap",
    packages=['PyComplexHeatmap'], #src
```

