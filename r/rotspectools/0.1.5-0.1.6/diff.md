# Comparing `tmp/rotspectools-0.1.5.tar.gz` & `tmp/rotspectools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotspectools-0.1.5.tar", max compression
+gzip compressed data, was "rotspectools-0.1.6.tar", max compression
```

## Comparing `rotspectools-0.1.5.tar` & `rotspectools-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-06-09 22:48:57.251928 rotspectools-0.1.5/LICENSE
--rw-r--r--   0        0        0     1754 2023-06-11 01:21:50.352482 rotspectools-0.1.5/README.rst
--rw-r--r--   0        0        0      459 2023-06-15 18:13:07.255869 rotspectools-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-06-10 00:31:55.788839 rotspectools-0.1.5/rotspectools/.DS_Store
--rw-r--r--   0        0        0      146 2023-06-15 18:12:39.518028 rotspectools-0.1.5/rotspectools/__init__.py
--rw-r--r--   0        0        0      414 2023-06-09 22:48:57.257324 rotspectools-0.1.5/rotspectools/cli.py
--rw-r--r--   0        0        0    29906 2023-06-15 18:05:26.747016 rotspectools-0.1.5/rotspectools/rotspectools.py
--rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 rotspectools-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-09 22:48:57.251928 rotspectools-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1754 2023-06-11 01:21:50.352482 rotspectools-0.1.6/README.rst
+-rw-r--r--   0        0        0      459 2023-06-16 00:42:55.668651 rotspectools-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-06-10 00:31:55.788839 rotspectools-0.1.6/rotspectools/.DS_Store
+-rw-r--r--   0        0        0      146 2023-06-16 00:42:40.976308 rotspectools-0.1.6/rotspectools/__init__.py
+-rw-r--r--   0        0        0      414 2023-06-09 22:48:57.257324 rotspectools-0.1.6/rotspectools/cli.py
+-rw-r--r--   0        0        0    25101 2023-06-16 00:39:18.680483 rotspectools-0.1.6/rotspectools/rotspectools.py
+-rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 rotspectools-0.1.6/PKG-INFO
```

### Comparing `rotspectools-0.1.5/LICENSE` & `rotspectools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.5/README.rst` & `rotspectools-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.5/rotspectools/.DS_Store` & `rotspectools-0.1.6/rotspectools/.DS_Store`

 * *Files identical despite different names*

### Comparing `rotspectools-0.1.5/rotspectools/rotspectools.py` & `rotspectools-0.1.6/rotspectools/rotspectools.py`

 * *Files 12% similar despite different names*

```diff
@@ -283,15 +283,15 @@
                 df_normal["Ka'"],
                 df_normal["J'"],
                 s=4 * df_normal["blend O-C/error"],
                 facecolors=df_normal["Transition Type"].map(
                     {
                         "a-type": "#0000FF65",
                         "b-type": "#00800045",
-                        "c-type": "#FFFFFF00",
+                        "c-type": "#FFA50020",
                     }
                 ),
                 edgecolors=df_normal["Transition Type"].map(
                     {"a-type": "blue", "b-type": "green", "c-type": "orange"}
                 ),
                 linewidth=0.8,
             )
@@ -315,15 +315,15 @@
             linewidth=0.8,
         )
         ax[1].scatter(
             df_normal_q["Ka'"],
             df_normal_q["J'"],
             s=4 * df_normal_q["blend O-C/error"],
             facecolors=df_normal_q["Transition Type"].map(
-                {"a-type": "#0000FF65", "b-type": "#00800045", "c-type": "#FFFFFF00"}
+                {"a-type": "#0000FF65", "b-type": "#00800045", "c-type": "#FFA50020"}
             ),
             edgecolors=df_normal_q["Transition Type"].map(
                 {"a-type": "blue", "b-type": "green", "c-type": "orange"}
             ),
             linewidth=0.8,
         )
 
@@ -412,29 +412,29 @@
         mpl.rc("text", usetex=True)
         plt.style.use(["science", "ieee"])
         self.categorize_error()
         self.res_dataframe = self.res_dataframe.sort_values(
             by=["Transition Type"], ascending=True
         )
         dataframes = self.split_branches()
-        dataframes = tuple(map(self.get_rot, dataframes))
+        dataframes = tuple(self.get_rot(x) for x in dataframes)
         fig, ax = plt.subplots(1, 2, figsize=(8, 4))
         for i in range(0, 2):
             condition = dataframes[i]["blend O-C/error"] >= 4
             df_high_error = dataframes[i][condition]
             df_normal = dataframes[i][~condition]
             ax[0].scatter(
                 df_normal["Ka'"],
                 df_normal["J'"],
                 s=4 * df_normal["blend O-C/error"],
                 facecolors=df_normal["Transition Type"].map(
                     {
                         "a-type": "#0000FF65",
                         "b-type": "#00800045",
-                        "c-type": "#FFFFFF00",
+                        "c-type": "#FFA50020",
                     }
                 ),
                 edgecolors=df_normal["Transition Type"].map(
                     {"a-type": "blue", "b-type": "green", "c-type": "orange"}
                 ),
                 linewidth=0.8,
             )
@@ -458,15 +458,15 @@
             linewidth=0.8,
         )
         ax[1].scatter(
             df_normal_q["Ka'"],
             df_normal_q["J'"],
             s=4 * df_normal_q["blend O-C/error"],
             facecolors=df_normal_q["Transition Type"].map(
-                {"a-type": "#0000FF65", "b-type": "#00800045", "c-type": "#FFFFFF00"}
+                {"a-type": "#0000FF65", "b-type": "#00800045", "c-type": "#FFA50020"}
             ),
             edgecolors=df_normal_q["Transition Type"].map(
                 {"a-type": "blue", "b-type": "green", "c-type": "orange"}
             ),
             linewidth=0.8,
         )
 
@@ -555,29 +555,29 @@
         mpl.rc("text", usetex=True)
         plt.style.use(["science", "ieee"])
         self.categorize_error()
         self.res_dataframe = self.res_dataframe.sort_values(
             by=["Transition Type"], ascending=True
         )
         dataframes = self.split_branches()
-        dataframes = tuple(map(self.get_IR, dataframes))
+        dataframes = tuple(self.get_IR(x) for x in dataframes)
         fig, ax = plt.subplots(1, 2, figsize=(8, 4))
         for i in range(0, 2):
             condition = dataframes[i]["blend O-C/error"] >= 4
             df_high_error = dataframes[i][condition]
             df_normal = dataframes[i][~condition]
             ax[0].scatter(
                 df_normal["Ka'"],
                 df_normal["J'"],
                 s=4 * df_normal["blend O-C/error"],
                 facecolors=df_normal["Transition Type"].map(
                     {
                         "a-type": "#0000FF65",
                         "b-type": "#00800045",
-                        "c-type": "#FFFFFF00",
+                        "c-type": "#FFA50020",
                     }
                 ),
                 edgecolors=df_normal["Transition Type"].map(
                     {"a-type": "blue", "b-type": "green", "c-type": "orange"}
                 ),
                 linewidth=0.8,
             )
@@ -601,15 +601,15 @@
             linewidth=0.8,
         )
         ax[1].scatter(
             df_normal_q["Ka'"],
             df_normal_q["J'"],
             s=4 * df_normal_q["blend O-C/error"],
             facecolors=df_normal_q["Transition Type"].map(
-                {"a-type": "#0000FF65", "b-type": "#00800045", "c-type": "#FFFFFF00"}
+                {"a-type": "#0000FF65", "b-type": "#00800045", "c-type": "#FFA50020"}
             ),
             edgecolors=df_normal_q["Transition Type"].map(
                 {"a-type": "blue", "b-type": "green", "c-type": "orange"}
             ),
             linewidth=0.8,
         )
 
@@ -690,150 +690,14 @@
             handler_map={mpatches.Circle: HandlerEllipse()},
         )
         frame1 = legend1.get_frame()
         frame1.set_linewidth(0.5)
         file_path = self.file_name + ".jpg"
         fig.savefig(file_path, dpi=800)
 
-    def plot_data_dist_notebook(self, max_Ka: int, max_J: int):
-        mpl.rcParams.update(mpl.rcParamsDefault)
-        self.categorize_error()
-        dataframes = self.split_lines()
-        fig, ax = plt.subplots(1, 2, figsize=(8, 4))
-        for i in range(0, 6):
-            condition = dataframes[i]["blend O-C/error"] >= 4
-            df_high_error = dataframes[i][condition]
-            df_normal = dataframes[i][~condition]
-            ax[0].scatter(
-                df_normal["Ka'"],
-                df_normal["J'"],
-                s=4 * df_normal["blend O-C/error"],
-                facecolors="white",
-                edgecolors=df_normal["Transition Type"].map(
-                    {"a-type": "#0000FF65", "b-type": "#00800045", "c-type": "orange"}
-                ),
-                linewidth=0.8,
-                alpha=0.5,
-            )
-            ax[0].scatter(
-                df_high_error["Ka'"],
-                df_high_error["J'"],
-                s=4 * df_high_error["blend O-C/error"],
-                facecolors="white",
-                edgecolors="red",
-                linewidth=0.8,
-                alpha=0.5,
-            )
-        for i in range(8, 5):
-            condition_q = dataframes[i]["blend O-C/error"] >= 4
-            df_high_error_q = dataframes[i][condition_q]
-            df_normal_q = dataframes[i][~condition_q]
-            ax[1].scatter(
-                df_high_error_q["Ka'"],
-                df_high_error_q["J'"],
-                s=4 * df_high_error_q["blend O-C/error"],
-                facecolors="white",
-                edgecolors="red",
-                linewidth=0.8,
-                alpha=0.5,
-            )
-            ax[1].scatter(
-                df_normal_q["Ka'"],
-                df_normal_q["J'"],
-                s=4 * df_normal_q["blend O-C/error"],
-                facecolors=df_normal_q["Transition Type"].map(
-                    {"a-type": "#0000FF65", "b-type": "#00800045", "c-type": "orange"}
-                ),
-                edgecolors=df_normal_q["Transition Type"].map(
-                    {"a-type": "#0000FF65", "b-type": "#00800045", "c-type": "orange"}
-                ),
-                alpha=0.5,
-                linewidth=0.8,
-            )
-
-        ax[0].axline((0, 0), slope=1, color="lightgrey", linewidth=1.5)
-        ax[0].set_xlabel("$K_a''$", fontsize=14)
-        ax[0].set_ylabel("$J''$", fontsize=14)
-        ax[0].set_ylim(0, max_J)
-        ax[0].set_xlim(-0.5, max_Ka)
-        ax[0].set_xticks((0, 10, 20, 30, 40, 50, 60))
-        ax[0].set_yticks((0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120))
-        ax[0].text(38, 110, "R-Branch", fontsize=18)
-
-        ax[1].axline((0, 0), slope=1, color="lightgrey", linewidth=1.5)
-        ax[1].set_xlabel("$K_a''$", fontsize=14)
-        ax[1].set_ylabel("$J''$", fontsize=14)
-        ax[1].set_ylim(0, max_J)
-        ax[1].set_xlim(-0.5, max_Ka)
-        ax[1].set_xticks((0, 10, 20, 30, 40, 50, 60))
-        ax[1].set_yticks((0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 110, 120))
-        ax[1].text(38, 110, "Q-Branch", fontsize=18)
-
-        c = [
-            mpatches.Circle(
-                (0.5, 0.5),
-                radius=0.25,
-                facecolor="#0000FF65",
-                edgecolor="none",
-                label="a-type",
-            ),
-            mpatches.Circle(
-                (0.5, 0.5),
-                radius=0.25,
-                facecolor="#00800045",
-                edgecolor="none",
-                label="b-type",
-            ),
-            mpatches.Circle(
-                (0.5, 0.5),
-                radius=0.25,
-                facecolor="orange",
-                edgecolor="none",
-                label="c-type",
-            ),
-            mpatches.Circle(
-                (0.5, 0.5),
-                radius=0.25,
-                facecolor="red",
-                edgecolor="none",
-                label=r"$>$ $3\sigma$",
-            ),
-        ]
-        texts = ["a-type", "b-type", "c-type", r"$>$ $3\sigma$"]
-        legend = ax[0].legend(
-            c,
-            texts,
-            loc="lower right",
-            fontsize=8,
-            frameon=True,
-            edgecolor="black",
-            framealpha=1,
-            borderaxespad=0,
-            fancybox=False,
-            handler_map={mpatches.Circle: HandlerEllipse()},
-        )
-        frame = legend.get_frame()
-        frame.set_linewidth(0.5)
-
-        legend1 = ax[1].legend(
-            c,
-            texts,
-            loc="lower right",
-            fontsize=8,
-            frameon=True,
-            edgecolor="black",
-            framealpha=1,
-            borderaxespad=0,
-            fancybox=False,
-            handler_map={mpatches.Circle: HandlerEllipse()},
-        )
-        frame1 = legend1.get_frame()
-        frame1.set_linewidth(0.5)
-        plt.show()
-
 
 class HandlerEllipse(HandlerPatch):
     def create_artists(
         self,
         legend,
         orig_handle,
         xdescent,
```

### Comparing `rotspectools-0.1.5/PKG-INFO` & `rotspectools-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotspectools
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 License: MIT
 Author: Dairen Jean
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

