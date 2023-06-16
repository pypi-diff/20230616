# Comparing `tmp/phdu-2.0b3.tar.gz` & `tmp/phdu-2.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-2.0b3.tar", last modified: Fri Jun 16 12:49:48 2023, max compression
+gzip compressed data, was "phdu-2.0b4.tar", last modified: Fri Jun 16 13:43:09 2023, max compression
```

## Comparing `phdu-2.0b3.tar` & `phdu-2.0b4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 12:49:48.803173 phdu-2.0b3/
--rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-2.0b3/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-06-16 12:49:48.803173 phdu-2.0b3/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-2.0b3/README.md
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 12:49:48.699168 phdu-2.0b3/phdu/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-2.0b3/phdu/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-2.0b3/phdu/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-2.0b3/phdu/clustering.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-2.0b3/phdu/decomposition.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-2.0b3/phdu/np_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-2.0b3/phdu/pd_utils.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 12:49:48.735169 phdu-2.0b3/phdu/plots/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-2.0b3/phdu/plots/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-2.0b3/phdu/plots/_mpl.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-2.0b3/phdu/plots/base.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    14316 2023-06-16 12:48:52.000000 phdu-2.0b3/phdu/plots/plotly_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-2.0b3/phdu/script_fmt.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 12:49:48.775171 phdu-2.0b3/phdu/stats/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-2.0b3/phdu/stats/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-2.0b3/phdu/stats/_integration.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-2.0b3/phdu/stats/_plots.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-2.0b3/phdu/stats/_preprocess.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    32364 2023-05-30 10:17:23.000000 phdu-2.0b3/phdu/stats/bootstrap.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-2.0b3/phdu/stats/conf_interval.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-2.0b3/phdu/stats/corr.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 12:49:48.783172 phdu-2.0b3/phdu/stats/rtopy/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-2.0b3/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-2.0b3/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-2.0b3/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 12:49:48.795172 phdu-2.0b3/phdu/stats/test/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-2.0b3/phdu/stats/test/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-2.0b3/phdu/stats/test/_adherence.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-2.0b3/phdu/stats/test/permutation.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4179 2023-04-25 11:08:38.000000 phdu-2.0b3/phdu/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 12:49:48.719169 phdu-2.0b3/phdu.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-06-16 12:49:48.000000 phdu-2.0b3/phdu.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-06-16 12:49:48.000000 phdu-2.0b3/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-06-16 12:49:48.000000 phdu-2.0b3/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-06-16 12:49:48.000000 phdu-2.0b3/phdu.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-06-16 12:49:48.000000 phdu-2.0b3/phdu.egg-info/top_level.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-06-16 12:49:48.811173 phdu-2.0b3/setup.cfg
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-06-16 12:49:24.000000 phdu-2.0b3/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 13:43:09.589052 phdu-2.0b4/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-2.0b4/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-06-16 13:43:09.589052 phdu-2.0b4/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-2.0b4/README.md
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 13:43:09.541050 phdu-2.0b4/phdu/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-2.0b4/phdu/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-2.0b4/phdu/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-2.0b4/phdu/clustering.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-2.0b4/phdu/decomposition.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-2.0b4/phdu/np_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-2.0b4/phdu/pd_utils.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 13:43:09.561051 phdu-2.0b4/phdu/plots/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-2.0b4/phdu/plots/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-2.0b4/phdu/plots/_mpl.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-2.0b4/phdu/plots/base.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    14956 2023-06-16 13:42:11.000000 phdu-2.0b4/phdu/plots/plotly_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-2.0b4/phdu/script_fmt.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 13:43:09.577052 phdu-2.0b4/phdu/stats/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-2.0b4/phdu/stats/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-2.0b4/phdu/stats/_integration.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-2.0b4/phdu/stats/_plots.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-2.0b4/phdu/stats/_preprocess.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    32364 2023-05-30 10:17:23.000000 phdu-2.0b4/phdu/stats/bootstrap.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-2.0b4/phdu/stats/conf_interval.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-2.0b4/phdu/stats/corr.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 13:43:09.581052 phdu-2.0b4/phdu/stats/rtopy/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-2.0b4/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-2.0b4/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-2.0b4/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 13:43:09.589052 phdu-2.0b4/phdu/stats/test/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-2.0b4/phdu/stats/test/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-2.0b4/phdu/stats/test/_adherence.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-2.0b4/phdu/stats/test/permutation.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4179 2023-04-25 11:08:38.000000 phdu-2.0b4/phdu/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 13:43:09.557051 phdu-2.0b4/phdu.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-06-16 13:43:09.000000 phdu-2.0b4/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-06-16 13:43:09.000000 phdu-2.0b4/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-06-16 13:43:09.000000 phdu-2.0b4/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-06-16 13:43:09.000000 phdu-2.0b4/phdu.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-06-16 13:43:09.000000 phdu-2.0b4/phdu.egg-info/top_level.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-06-16 13:43:09.593052 phdu-2.0b4/setup.cfg
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-06-16 13:42:45.000000 phdu-2.0b4/setup.py
```

### Comparing `phdu-2.0b3/LICENSE.md` & `phdu-2.0b4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/PKG-INFO` & `phdu-2.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.0b3
+Version: 2.0b4
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.0b3/README.md` & `phdu-2.0b4/README.md`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu/_helper.py` & `phdu-2.0b4/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu/clustering.py` & `phdu-2.0b4/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu/decomposition.py` & `phdu-2.0b4/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu/np_utils.py` & `phdu-2.0b4/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu/pd_utils.py` & `phdu-2.0b4/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu/plots/base.py` & `phdu-2.0b4/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu/plots/plotly_utils.py` & `phdu-2.0b4/phdu/plots/plotly_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -149,29 +149,33 @@
     Attributes:
         - x:    x coordinate for the CI
         - y:    value of the magnitude for the sample. Example: the mean if CI is a CI for the mean.
         - CI:   Confidence interval for y.
     """
     if fig is None:
         fig = get_figure(xaxis_title=x_title, yaxis_title=y_title)
+
+    idx_to_xlabel = {i: x_val for i, x_val in enumerate(x)}
     for i, (ci, x_val, ci_stat) in enumerate(zip(CI, x, y)):
         if not np.isnan(ci).all():
-            fig.add_shape(type="line", xref="x", yref="y", line=dict(color=color_sample_stat, width=width_sample_stat),  x0=i-width, y0=ci_stat, x1=i+width, y1=ci_stat)
             fig.add_shape(type="rect", xref="x", yref="y", line=dict(color="gray",width=4), fillcolor=color, x0=i-width, y0=ci[0], x1=i+width, y1=ci[1])
-            fig.add_trace(go.Scatter(x=[x_val]*2, y=ci[::-1], showlegend=False, mode="markers",
+            fig.add_trace(go.Scatter(x=[i]*2, y=ci[::-1], showlegend=False, mode="markers",
                                      marker=dict(color=color, symbol=["arrow-bar-down", "arrow-bar-up"], size=ms, line=dict(color="gray", width=2))
                                 ))
+            fig.add_shape(type="line", xref="x", yref="y", line=dict(color=color_sample_stat, width=width_sample_stat),  x0=i-width, y0=ci_stat, x1=i+width, y1=ci_stat)
+
+        fig.update_layout(xaxis=dict(tickvals=[*idx_to_xlabel.keys()], ticktext=[*idx_to_xlabel.values()]))
     if label is not None:
         yrange = [*get_common_range(fig, axes=["y"]).values()][0]
         fig.add_trace(go.Scatter(x=[1000], y=[1000], mode="markers", name=label, showlegend=True,
                                  marker=dict(symbol="square", color=color, size=22), line=dict(color="gray", width=2)))
         fig.update_layout(**mod_range(fig, ([-0.25, len(x)-0.75], yrange)))
     return fig
 
-def CI_ss_plot(df, label=False, width=0.05, ms=10, ns_color='#323232', ss_lower_color='#1f77b4', ss_upper_color='#ff7f0e', **CI_plot_kwargs):
+def CI_ss_plot(df, label=False, width=0.05, ms=10, ns_color='#323232', ss_lower_color='#1f77b4', ss_upper_color='#ff7f0e', color_sample_stat='black', width_sample_stat=5, **CI_plot_kwargs):
     """
     df: Dataframe containing the x coordinate in the index
         and columns:
             - 'sample stat': sample statistic
             - 'CI':          confidence interval
             - 'lb':          lower bound
             - 'ub':          upper bound
@@ -187,19 +191,20 @@
     df_ns, df_ss_upper, df_ss_lower = df.copy(), df.copy(), df.copy()
     cis = np.vstack(df.CI.values)
     df_ns['CI'] = map_to_nan(cis, ss).tolist()
     df_ss_upper['CI'] = map_to_nan(cis, ~ss_upper).tolist()
     df_ss_lower['CI'] = map_to_nan(cis, ~ss_lower).tolist()
     # NS intervals
     fig = CI_plot(df_ns.index, df_ns['sample stat'].values, np.vstack(df_ns['CI'].values), width=width, ms=ms, color=color_std(ns_color, opacity=0.55), label='Not SS' if label else None,
+                  color_sample_stat=color_sample_stat, width_sample_stat=width_sample_stat,
                   **CI_plot_kwargs)
     # Adding significant intervals
     figdata = {'SS (>0)': (df_ss_upper, ss_upper_color), 'SS (<0)': (df_ss_lower, ss_lower_color)}
     for label_ss, (df_ss, ss_color) in figdata.items():
-        fig = CI_plot(df_ss.index, df_ss['sample stat'].values, np.vstack(df_ss['CI'].values), width=width, ms=ms, fig=fig, color=color_std(ss_color, opacity=0.2), label=label_ss if label else None)
+        fig = CI_plot(df_ss.index, df_ss['sample stat'].values, np.vstack(df_ss['CI'].values), width=width, ms=ms, fig=fig, color=color_std(ss_color, opacity=0.2), label=label_ss if label else None, color_sample_stat=color_sample_stat, width_sample_stat=width_sample_stat)
     # colorizing the index
     def colorize(index_upper, index_lower):
         """
         index: pd.Series where index is the feature name and value is of type bool.
         """
         ticktext = []
         for f, is_ss_upper in index_upper.items():
@@ -208,14 +213,18 @@
             elif index_lower[f]: # is_ss_lower
                 ticktext.append(f"<span style='color:{str(ss_lower_color)}'> {str(f)} </span>")
             else:
                 ticktext.append(f"<span style='color:{str(ns_color)}'> {str(f)} </span>")
         return ticktext
     ticktext = colorize(ss_upper, ss_lower)
     fig.update_layout(xaxis=dict(tickmode='array', ticktext=ticktext, tickvals=np.arange(ss.size)))
+
+    fig.update_layout(plot_bgcolor='white', yaxis=dict(showline=True, linecolor='black', linewidth=2.4),
+                      xaxis=dict(showline=True, linecolor='black', linewidth=2.4))
+    fig.add_hline(y=0, line=dict(color='black', width=1, dash='dash'))
     return fig
 
 def permtest_plot(df, H1="", colorscale="Inferno", log=True, height=800, width=1000, font_size=40, bar_len=0.9, bar_x=0.95, bar_thickness=100):
     """H1 should not contain latex code. Use unicode and HTML for super/sub-indices."""
     if log:
         df = np.log10(df)
         zmin, zmax = np.log10(0.05), 0
```

### Comparing `phdu-2.0b3/phdu/script_fmt.py` & `phdu-2.0b4/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu/stats/_integration.py` & `phdu-2.0b4/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu/stats/_plots.py` & `phdu-2.0b4/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu/stats/bootstrap.py` & `phdu-2.0b4/phdu/stats/bootstrap.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu/stats/conf_interval.py` & `phdu-2.0b4/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu/stats/corr.py` & `phdu-2.0b4/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu/stats/rtopy/_helper.py` & `phdu-2.0b4/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu/stats/rtopy/resample.py` & `phdu-2.0b4/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu/stats/test/permutation.py` & `phdu-2.0b4/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu/storage.py` & `phdu-2.0b4/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/phdu.egg-info/PKG-INFO` & `phdu-2.0b4/phdu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.0b3
+Version: 2.0b4
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.0b3/phdu.egg-info/SOURCES.txt` & `phdu-2.0b4/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-2.0b3/setup.py` & `phdu-2.0b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='2.0.b3',
+    version='2.0.b4',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```

