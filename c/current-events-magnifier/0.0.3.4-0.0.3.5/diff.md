# Comparing `tmp/current_events_magnifier-0.0.3.4.tar.gz` & `tmp/current_events_magnifier-0.0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/current_events_magnifier-0.0.3.4.tar", last modified: Thu Jun 15 10:47:22 2023, max compression
+gzip compressed data, was "current_events_magnifier-0.0.3.5.tar", last modified: Fri Jun 16 08:59:42 2023, max compression
```

## Comparing `current_events_magnifier-0.0.3.4.tar` & `current_events_magnifier-0.0.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 10:47:22.369872 current_events_magnifier-0.0.3.4/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.3.4/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6020 2023-06-15 10:47:22.369872 current_events_magnifier-0.0.3.4/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5408 2023-06-14 11:16:12.000000 current_events_magnifier-0.0.3.4/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 10:47:22.365872 current_events_magnifier-0.0.3.4/current_events_magnifier/
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     6268 2023-06-15 02:13:38.000000 current_events_magnifier-0.0.3.4/current_events_magnifier/CE_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 12:01:39.000000 current_events_magnifier-0.0.3.4/current_events_magnifier/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.3.4/current_events_magnifier/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.3.4/current_events_magnifier/cem_utils.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.3.4/current_events_magnifier/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7556 2023-06-14 11:49:38.000000 current_events_magnifier-0.0.3.4/current_events_magnifier/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.0.3.4/current_events_magnifier/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13168 2023-06-14 12:00:50.000000 current_events_magnifier-0.0.3.4/current_events_magnifier/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 10:47:22.365872 current_events_magnifier-0.0.3.4/current_events_magnifier.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6020 2023-06-15 10:47:22.000000 current_events_magnifier-0.0.3.4/current_events_magnifier.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      600 2023-06-15 10:47:22.000000 current_events_magnifier-0.0.3.4/current_events_magnifier.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-15 10:47:22.000000 current_events_magnifier-0.0.3.4/current_events_magnifier.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       98 2023-06-15 10:47:22.000000 current_events_magnifier-0.0.3.4/current_events_magnifier.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-15 10:47:22.000000 current_events_magnifier-0.0.3.4/current_events_magnifier.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-15 10:47:22.369872 current_events_magnifier-0.0.3.4/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1094 2023-06-15 10:47:20.000000 current_events_magnifier-0.0.3.4/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-16 08:59:42.875690 current_events_magnifier-0.0.3.5/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.3.5/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5996 2023-06-16 08:59:42.875690 current_events_magnifier-0.0.3.5/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5341 2023-06-16 08:59:37.000000 current_events_magnifier-0.0.3.5/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-16 08:59:42.875690 current_events_magnifier-0.0.3.5/current_events_magnifier/
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     6317 2023-06-16 08:57:45.000000 current_events_magnifier-0.0.3.5/current_events_magnifier/CE_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6737 2023-06-16 08:57:45.000000 current_events_magnifier-0.0.3.5/current_events_magnifier/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.3.5/current_events_magnifier/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.3.5/current_events_magnifier/cem_utils.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.3.5/current_events_magnifier/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7625 2023-06-16 08:56:20.000000 current_events_magnifier-0.0.3.5/current_events_magnifier/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.0.3.5/current_events_magnifier/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13168 2023-06-14 12:00:50.000000 current_events_magnifier-0.0.3.5/current_events_magnifier/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-16 08:59:42.875690 current_events_magnifier-0.0.3.5/current_events_magnifier.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5996 2023-06-16 08:59:42.000000 current_events_magnifier-0.0.3.5/current_events_magnifier.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      600 2023-06-16 08:59:42.000000 current_events_magnifier-0.0.3.5/current_events_magnifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-16 08:59:42.000000 current_events_magnifier-0.0.3.5/current_events_magnifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       98 2023-06-16 08:59:42.000000 current_events_magnifier-0.0.3.5/current_events_magnifier.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-16 08:59:42.000000 current_events_magnifier-0.0.3.5/current_events_magnifier.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-16 08:59:42.875690 current_events_magnifier-0.0.3.5/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1100 2023-06-16 08:59:37.000000 current_events_magnifier-0.0.3.5/setup.py
```

### Comparing `current_events_magnifier-0.0.3.4/LICENSE` & `current_events_magnifier-0.0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.4/PKG-INFO` & `current_events_magnifier-0.0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: current_events_magnifier
-Version: 0.0.3.4
+Version: 0.0.3.5
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Current_Magnifier
 `Current_Magnifier` is a sample tool designed to visualize the features(Mean,Median,Dwell_time,STD) that distinguish between two groups of ONT data from the same species at the site level.
 It supports two re-squiggle pipeline(`Tombo` and `f5c`). From R9 to R10, Tombo/nanopolish/f5c applied different method to optimise the alignment. So, this program can examine the differences in the current generated by ONT at the same site across multiple dimensions, making it easier for researchers to showcase and demonstrate their discoveries of mutations and modifications.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
@@ -33,23 +35,22 @@
 This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
 Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but  resquiggle is a more fine alignment than the move table in most cases.
 
 ## Installation
 Requirement : Python >=3.7
 
 ```sh
-git clone git@github.com:lrslab/Current_Magnifier.git
-cd Current_Magnifier/
-pip install -r requirements.txt
+pip install current_events_magnifier==0.0.3.5
+
 conda install -c bioconda ont_vbz_hdf_plugin
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
-python CE_magnifier.py tombo -h
+ CE_magnifier.py tombo -h
 optional arguments:
   -h, --help            show this help message and exit
   --basecall_group BASECALL_GROUP
                         The attribute group to extract the training data from. e.g. RawGenomeCorrected_000
   --basecall_subgroup BASECALL_SUBGROUP
                         Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template
   -i FAST5, --fast5 FAST5
@@ -124,7 +125,9 @@
 
 ```
 
 
 
 
 
+
+
```

### Comparing `current_events_magnifier-0.0.3.4/README.md` & `current_events_magnifier-0.0.3.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,22 @@
 This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
 Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but  resquiggle is a more fine alignment than the move table in most cases.
 
 ## Installation
 Requirement : Python >=3.7
 
 ```sh
-git clone git@github.com:lrslab/Current_Magnifier.git
-cd Current_Magnifier/
-pip install -r requirements.txt
+pip install current_events_magnifier==0.0.3.5
+
 conda install -c bioconda ont_vbz_hdf_plugin
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
-python CE_magnifier.py tombo -h
+ CE_magnifier.py tombo -h
 optional arguments:
   -h, --help            show this help message and exit
   --basecall_group BASECALL_GROUP
                         The attribute group to extract the training data from. e.g. RawGenomeCorrected_000
   --basecall_subgroup BASECALL_SUBGROUP
                         Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template
   -i FAST5, --fast5 FAST5
```

### Comparing `current_events_magnifier-0.0.3.4/current_events_magnifier/CE_magnifier.py` & `current_events_magnifier-0.0.3.5/current_events_magnifier/CE_magnifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,11 +110,12 @@
 
     category_data = [str(args.pos + x) for x in range(-args.len, args.len + 1)]
     category = pd.api.types.CategoricalDtype(categories=category_data, ordered=True)
     df['position'] = df['position'].astype(category)
 
     # draw_volin(df,results_path,args.pos,base_list,title)
     # draw_boxplot(df,results_path,args.pos,base_list,title)
+    print("Start to generate plots and save  in "+ results_path)
     signal_plot(df, results_path, args.pos, base_list, title, 'merged')
     signal_plot(df, results_path, args.pos, base_list, title, 'boxplot')
     signal_plot(df, results_path, args.pos, base_list, title, 'violin_plot')
-    print('\nsaved as ', args.output)
+    print('finished')
```

### Comparing `current_events_magnifier-0.0.3.4/current_events_magnifier/cem_utils.py` & `current_events_magnifier-0.0.3.5/current_events_magnifier/cem_utils.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.4/current_events_magnifier/normalization.py` & `current_events_magnifier-0.0.3.5/current_events_magnifier/normalization.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.4/current_events_magnifier/plot.py` & `current_events_magnifier-0.0.3.5/current_events_magnifier/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import pandas as pd
 import plotnine as p9
 import numpy as np
 from matplotlib import pyplot as plt
+
 plt.rcParams['pdf.fonttype'] = 42
 # plt.rcParams['font.sans-serif'] = ['Arial']
 SIG_PCTL_RANGE = (2.5, 97.5)
+
+
 # def draw_boxplot(df,results_path,pos,base_list,title):
 #     item_list = ['Mean', 'STD', 'Median', 'Dwell_time']
 #     plot_list=[]
 #     for item in item_list:
 #
 #         sig_min, sig_max = np.percentile(df[item], SIG_PCTL_RANGE)
 #         sig_diff = sig_max - sig_min
@@ -54,19 +57,19 @@
 #             legend_position='none'
 #         )\
 #         + p9.ylim(ylim_tuple)
 #
 #         plot = plot + p9.labs(title=title, x=str(pos + 1), y=item)
 #         # plot.render_matplotlib()
 #         plot.save(filename=results_path + "/" + item + "_violin.pdf", dpi=300)
-        # print(plot)
+# print(plot)
 
-def signal_plot(df,results_path,pos,base_list,title,plot_type):
+def signal_plot(df, results_path, pos, base_list, title, plot_type):
     item_list = ['Mean', 'STD', 'Median', 'Dwell time']
-    if plot_type !='merged':
+    if plot_type != 'merged':
 
         for item in item_list:
             sig_min, sig_max = np.percentile(df[item], SIG_PCTL_RANGE)
             sig_diff = sig_max - sig_min
             ylim_tuple = (sig_min - sig_diff * 0.1, sig_max + sig_diff * 0.1)
 
             plot = p9.ggplot(df, p9.aes(x='position', y=item, fill='type')) \
@@ -76,43 +79,43 @@
                    + p9.theme(
                 figure_size=(6, 3),
                 panel_grid_minor=p9.element_blank(),
                 axis_text=p9.element_text(size=13),
                 axis_title=p9.element_text(size=13),
                 title=p9.element_text(size=13),
                 legend_position='none'
-            )\
-            + p9.ylim(ylim_tuple)
+            ) \
+                   + p9.ylim(ylim_tuple)
             plot = plot + p9.labs(title=title, x=str(pos + 1), y=item)
             if plot_type == 'boxplot':
-                plot = plot + p9.geom_boxplot( outlier_shape='',position=p9.position_dodge(0.9),size=0.25)
+                plot = plot + p9.geom_boxplot(outlier_shape='', position=p9.position_dodge(0.9), size=0.25)
             elif plot_type == 'violin_plot':
-                plot = plot + p9.geom_violin(style='left-right',position=p9.position_dodge(0),color='none',width=1.5)
+                plot = plot + p9.geom_violin(style='left-right', position=p9.position_dodge(0), color='none', width=1.5)
             else:
                 raise Exception("Unsupported figure type!")
             # plot.render_matplotlib()
-            if item=='Dwell time':
-                item='Dwell_time'
-            plot.save(filename=results_path + "/" + item + "_"+plot_type+".pdf", dpi=300)
+            if item == 'Dwell time':
+                item = 'Dwell_time'
+            plot.save(filename=results_path + "/" + item + "_" + plot_type + ".pdf", dpi=300)
     else:
-        new_df=None
+        new_df = None
         for item in item_list:
             # collect data
-            temp= df[[item,'position','type']]
-            temp.columns=['value','position','type']
-            temp['stats']=item
+            temp = df[[item, 'position', 'type']].copy()
+            temp.columns = ['value', 'position', 'type']
+            temp.loc[:, 'stats'] = item
 
             sig_min, sig_max = np.percentile(temp['value'], SIG_PCTL_RANGE)
             sig_diff = sig_max - sig_min
             ylim_tuple = [sig_min - sig_diff * 0.1, sig_max + sig_diff * 0.1]
-            temp = temp[(temp['value']>= ylim_tuple[0]) & (temp['value']<= ylim_tuple[1]) ]
+            temp = temp[(temp['value'] >= ylim_tuple[0]) & (temp['value'] <= ylim_tuple[1])]
             if new_df is None:
                 new_df = temp
             else:
-                new_df=pd.concat([new_df,temp],axis=0)
+                new_df = pd.concat([new_df, temp], axis=0)
 
         plot = p9.ggplot(new_df, p9.aes(x='position', y="value", fill='type')) \
                + p9.theme_bw() \
                + p9.scale_fill_manual(values={"Sample": "#ff6f91", "Control": "#7389af", "Single": "#a3abbd"}) \
                + p9.scale_x_discrete(labels=list(base_list)) \
                + p9.theme(
             figure_size=(8, 8),
@@ -123,41 +126,42 @@
             strip_text=p9.element_text(size=13),
             legend_position='none',
             strip_background=p9.element_rect(alpha=0)
         ) \
                + p9.facet_grid('stats ~', scales='free_y')
         plot = plot + p9.labs(title=title, x=str(pos + 1), y='')
 
-        if new_df['type'].drop_duplicates().shape[0]==1:
-            plot2 = plot + p9.geom_violin(color='none', position=p9.position_dodge(0.9),width=1)
+        if new_df['type'].drop_duplicates().shape[0] == 1:
+            plot2 = plot + p9.geom_violin(color='none', position=p9.position_dodge(0.9), width=1)
             plot2 = plot2 + p9.geom_boxplot(outlier_shape='', position=p9.position_dodge(0.9), size=0.2, width=0.1)
             plot2.save(filename=results_path + "/merged_single.pdf", dpi=300)
         else:
             plot1 = plot + p9.geom_boxplot(outlier_shape='', position=p9.position_dodge(0.9), size=0.2, width=0.75)
             plot1.save(filename=results_path + "/merged_boxplot.pdf", dpi=300)
-            plot2 = plot + p9.geom_violin(style='left-right',position=p9.position_dodge(0),color='none',width=1.5)
+            plot2 = plot + p9.geom_violin(style='left-right', position=p9.position_dodge(0), color='none', width=1.5)
             plot2.save(filename=results_path + "/merged_violin.pdf", dpi=300)
 
-def draw_signal(df,start,base):
-    df=pd.DataFrame(df)
-    df.columns=['raw']
+
+def draw_signal(df, start, base):
+    df = pd.DataFrame(df)
+    df.columns = ['raw']
     df = df.reset_index()
     plot = p9.ggplot(df, p9.aes(x='index', y="raw")) \
            + p9.theme_bw() \
-            + p9.geom_line()\
+           + p9.geom_line() \
            + p9.theme(
         figure_size=(6, 3),
         panel_grid_minor=p9.element_blank(),
         axis_text=p9.element_text(size=13),
         axis_title=p9.element_text(size=13),
         title=p9.element_text(size=13),
         strip_text=p9.element_text(size=13),
         legend_position='none',
         strip_background=p9.element_rect(alpha=0)
     )
     # plot.save(filename="/home/zhguo/Dropbox/@labfiles/projects/GUO/ONT_showcase_tool/plot/signal.pdf", dpi=300)
     for item in start:
-        plot=plot+p9.geom_vline(xintercept=item, linetype='dashed', color='red')
+        plot = plot + p9.geom_vline(xintercept=item, linetype='dashed', color='red')
     print(base)
     # plot.save(filename="/home/zhguo/Dropbox/@labfiles/projects/GUO/ONT_showcase_tool/plot/norm_signal_aligned.pdf", dpi=300)
 
-    print(1)
+    print(1)
```

### Comparing `current_events_magnifier-0.0.3.4/current_events_magnifier/read_f5c_resquiggle.py` & `current_events_magnifier-0.0.3.5/current_events_magnifier/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.4/current_events_magnifier/read_tombo_resquiggle.py` & `current_events_magnifier-0.0.3.5/current_events_magnifier/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.4/current_events_magnifier.egg-info/PKG-INFO` & `current_events_magnifier-0.0.3.5/current_events_magnifier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: current-events-magnifier
-Version: 0.0.3.4
+Version: 0.0.3.5
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Current_Magnifier
 `Current_Magnifier` is a sample tool designed to visualize the features(Mean,Median,Dwell_time,STD) that distinguish between two groups of ONT data from the same species at the site level.
 It supports two re-squiggle pipeline(`Tombo` and `f5c`). From R9 to R10, Tombo/nanopolish/f5c applied different method to optimise the alignment. So, this program can examine the differences in the current generated by ONT at the same site across multiple dimensions, making it easier for researchers to showcase and demonstrate their discoveries of mutations and modifications.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
@@ -33,23 +35,22 @@
 This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
 Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but  resquiggle is a more fine alignment than the move table in most cases.
 
 ## Installation
 Requirement : Python >=3.7
 
 ```sh
-git clone git@github.com:lrslab/Current_Magnifier.git
-cd Current_Magnifier/
-pip install -r requirements.txt
+pip install current_events_magnifier==0.0.3.5
+
 conda install -c bioconda ont_vbz_hdf_plugin
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
-python CE_magnifier.py tombo -h
+ CE_magnifier.py tombo -h
 optional arguments:
   -h, --help            show this help message and exit
   --basecall_group BASECALL_GROUP
                         The attribute group to extract the training data from. e.g. RawGenomeCorrected_000
   --basecall_subgroup BASECALL_SUBGROUP
                         Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template
   -i FAST5, --fast5 FAST5
@@ -124,7 +125,9 @@
 
 ```
 
 
 
 
 
+
+
```

### Comparing `current_events_magnifier-0.0.3.4/current_events_magnifier.egg-info/SOURCES.txt` & `current_events_magnifier-0.0.3.5/current_events_magnifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.3.4/setup.py` & `current_events_magnifier-0.0.3.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="current_events_magnifier",
-    version="0.0.3.4",
+    version="0.0.3.5",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.7,<3.10',
     install_requires=[
         'h5py==3.8.0',
         'numpy>=1.23.0',
         'pandas>=1.1.5',
         'plotnine>=0.8.0',
         'tqdm>=4.62.0',
         "pysam>=0.21.0",
```

