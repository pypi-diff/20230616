# Comparing `tmp/phdu-2.0b2.tar.gz` & `tmp/phdu-2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-2.0b2.tar", last modified: Tue May 30 10:18:04 2023, max compression
+gzip compressed data, was "phdu-2.0b3.tar", last modified: Fri Jun 16 12:49:48 2023, max compression
```

## Comparing `phdu-2.0b2.tar` & `phdu-2.0b3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-30 10:18:04.720690 phdu-2.0b2/
--rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-2.0b2/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-05-30 10:18:04.720690 phdu-2.0b2/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-2.0b2/README.md
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-30 10:18:04.628686 phdu-2.0b2/phdu/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-2.0b2/phdu/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-2.0b2/phdu/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-2.0b2/phdu/clustering.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-2.0b2/phdu/decomposition.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-2.0b2/phdu/np_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-2.0b2/phdu/pd_utils.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-30 10:18:04.672688 phdu-2.0b2/phdu/plots/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-2.0b2/phdu/plots/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-2.0b2/phdu/plots/_mpl.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-2.0b2/phdu/plots/base.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    14228 2023-05-09 13:23:15.000000 phdu-2.0b2/phdu/plots/plotly_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-2.0b2/phdu/script_fmt.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-30 10:18:04.696689 phdu-2.0b2/phdu/stats/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-2.0b2/phdu/stats/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-2.0b2/phdu/stats/_integration.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-2.0b2/phdu/stats/_plots.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-2.0b2/phdu/stats/_preprocess.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    32364 2023-05-30 10:17:23.000000 phdu-2.0b2/phdu/stats/bootstrap.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-2.0b2/phdu/stats/conf_interval.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-2.0b2/phdu/stats/corr.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-30 10:18:04.704690 phdu-2.0b2/phdu/stats/rtopy/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-2.0b2/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-2.0b2/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-2.0b2/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-30 10:18:04.716690 phdu-2.0b2/phdu/stats/test/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-2.0b2/phdu/stats/test/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-2.0b2/phdu/stats/test/_adherence.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-2.0b2/phdu/stats/test/permutation.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4179 2023-04-25 11:08:38.000000 phdu-2.0b2/phdu/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-05-30 10:18:04.656687 phdu-2.0b2/phdu.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-05-30 10:18:04.000000 phdu-2.0b2/phdu.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-05-30 10:18:04.000000 phdu-2.0b2/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-05-30 10:18:04.000000 phdu-2.0b2/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-05-30 10:18:04.000000 phdu-2.0b2/phdu.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-05-30 10:18:04.000000 phdu-2.0b2/phdu.egg-info/top_level.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-05-30 10:18:04.728691 phdu-2.0b2/setup.cfg
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-05-30 10:17:46.000000 phdu-2.0b2/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 12:49:48.803173 phdu-2.0b3/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-2.0b3/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-06-16 12:49:48.803173 phdu-2.0b3/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-2.0b3/README.md
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 12:49:48.699168 phdu-2.0b3/phdu/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      486 2023-03-07 15:15:16.000000 phdu-2.0b3/phdu/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      608 2023-02-14 14:36:41.000000 phdu-2.0b3/phdu/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2828 2023-03-16 13:46:54.000000 phdu-2.0b3/phdu/clustering.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-2.0b3/phdu/decomposition.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2628 2023-02-14 17:21:31.000000 phdu-2.0b3/phdu/np_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     5912 2023-03-16 10:33:06.000000 phdu-2.0b3/phdu/pd_utils.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 12:49:48.735169 phdu-2.0b3/phdu/plots/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-2.0b3/phdu/plots/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-2.0b3/phdu/plots/_mpl.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3359 2022-11-09 08:55:15.000000 phdu-2.0b3/phdu/plots/base.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    14316 2023-06-16 12:48:52.000000 phdu-2.0b3/phdu/plots/plotly_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-2.0b3/phdu/script_fmt.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 12:49:48.775171 phdu-2.0b3/phdu/stats/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-2.0b3/phdu/stats/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-2.0b3/phdu/stats/_integration.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-2.0b3/phdu/stats/_plots.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-2.0b3/phdu/stats/_preprocess.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    32364 2023-05-30 10:17:23.000000 phdu-2.0b3/phdu/stats/bootstrap.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-2.0b3/phdu/stats/conf_interval.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-2.0b3/phdu/stats/corr.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 12:49:48.783172 phdu-2.0b3/phdu/stats/rtopy/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-2.0b3/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-2.0b3/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-2.0b3/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 12:49:48.795172 phdu-2.0b3/phdu/stats/test/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-2.0b3/phdu/stats/test/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-2.0b3/phdu/stats/test/_adherence.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-2.0b3/phdu/stats/test/permutation.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4179 2023-04-25 11:08:38.000000 phdu-2.0b3/phdu/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-06-16 12:49:48.719169 phdu-2.0b3/phdu.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2023-06-16 12:49:48.000000 phdu-2.0b3/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      752 2023-06-16 12:49:48.000000 phdu-2.0b3/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-06-16 12:49:48.000000 phdu-2.0b3/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2023-06-16 12:49:48.000000 phdu-2.0b3/phdu.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2023-06-16 12:49:48.000000 phdu-2.0b3/phdu.egg-info/top_level.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-06-16 12:49:48.811173 phdu-2.0b3/setup.cfg
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1660 2023-06-16 12:49:24.000000 phdu-2.0b3/setup.py
```

### Comparing `phdu-2.0b2/LICENSE.md` & `phdu-2.0b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/PKG-INFO` & `phdu-2.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.0b2
+Version: 2.0b3
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.0b2/README.md` & `phdu-2.0b3/README.md`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu/_helper.py` & `phdu-2.0b3/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu/clustering.py` & `phdu-2.0b3/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu/decomposition.py` & `phdu-2.0b3/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu/np_utils.py` & `phdu-2.0b3/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu/pd_utils.py` & `phdu-2.0b3/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu/plots/base.py` & `phdu-2.0b3/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu/plots/plotly_utils.py` & `phdu-2.0b3/phdu/plots/plotly_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,32 +138,32 @@
 
 def set_multicategory_from_df(fig, df):
     fig.update_layout(xaxis_type="multicategory", yaxis_type="multicategory")
     fig.data[0]["x"] = multiindex_to_label(df.columns)
     fig.data[0]["y"] = multiindex_to_label(df.index)
     return
 
-def CI_plot(x, y, CI, label=None, width=0.05, ms=10, color='rgba(255, 127, 14, 0.3)', fig=None, x_title=None, y_title=None):
+def CI_plot(x, y, CI, label=None, width=0.05, ms=10, color='rgba(255, 127, 14, 0.3)', color_sample_stat="green", width_sample_stat=8,  fig=None, x_title=None, y_title=None):
     """
     Box plot where the box corresponds to the CI.
 
     Attributes:
         - x:    x coordinate for the CI
         - y:    value of the magnitude for the sample. Example: the mean if CI is a CI for the mean.
         - CI:   Confidence interval for y.
     """
     if fig is None:
         fig = get_figure(xaxis_title=x_title, yaxis_title=y_title)
     for i, (ci, x_val, ci_stat) in enumerate(zip(CI, x, y)):
-        fig.add_trace(go.Scatter(x=[x_val]*2, y=ci[::-1], showlegend=False, mode="markers",
-                                 marker=dict(color=color, symbol=["arrow-bar-down", "arrow-bar-up"], size=ms, line=dict(color="gray", width=2))
-                                ))
         if not np.isnan(ci).all():
-            fig.add_shape(type="rect", xref="x", yref="y", line=dict(color="gray",width=3), fillcolor=color, x0=i-width, y0=ci[0], x1=i+width, y1=ci[1])
-        fig.add_shape(type="line", xref="x", yref="y", line=dict(color="gray", width=4),  x0=i-width, y0=ci_stat, x1=i+width, y1=ci_stat)
+            fig.add_shape(type="line", xref="x", yref="y", line=dict(color=color_sample_stat, width=width_sample_stat),  x0=i-width, y0=ci_stat, x1=i+width, y1=ci_stat)
+            fig.add_shape(type="rect", xref="x", yref="y", line=dict(color="gray",width=4), fillcolor=color, x0=i-width, y0=ci[0], x1=i+width, y1=ci[1])
+            fig.add_trace(go.Scatter(x=[x_val]*2, y=ci[::-1], showlegend=False, mode="markers",
+                                     marker=dict(color=color, symbol=["arrow-bar-down", "arrow-bar-up"], size=ms, line=dict(color="gray", width=2))
+                                ))
     if label is not None:
         yrange = [*get_common_range(fig, axes=["y"]).values()][0]
         fig.add_trace(go.Scatter(x=[1000], y=[1000], mode="markers", name=label, showlegend=True,
                                  marker=dict(symbol="square", color=color, size=22), line=dict(color="gray", width=2)))
         fig.update_layout(**mod_range(fig, ([-0.25, len(x)-0.75], yrange)))
     return fig
```

### Comparing `phdu-2.0b2/phdu/script_fmt.py` & `phdu-2.0b3/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu/stats/_integration.py` & `phdu-2.0b3/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu/stats/_plots.py` & `phdu-2.0b3/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu/stats/bootstrap.py` & `phdu-2.0b3/phdu/stats/bootstrap.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu/stats/conf_interval.py` & `phdu-2.0b3/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu/stats/corr.py` & `phdu-2.0b3/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu/stats/rtopy/_helper.py` & `phdu-2.0b3/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu/stats/rtopy/resample.py` & `phdu-2.0b3/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu/stats/test/permutation.py` & `phdu-2.0b3/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu/storage.py` & `phdu-2.0b3/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/phdu.egg-info/PKG-INFO` & `phdu-2.0b3/phdu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.0b2
+Version: 2.0b3
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.0b2/phdu.egg-info/SOURCES.txt` & `phdu-2.0b3/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-2.0b2/setup.py` & `phdu-2.0b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='2.0.b2',
+    version='2.0.b3',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```

