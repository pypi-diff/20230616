# Comparing `tmp/catencfamily-0.0.75.tar.gz` & `tmp/catencfamily-0.0.76.tar.gz`

## Comparing `catencfamily-0.0.75.tar` & `catencfamily-0.0.76.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.75/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.75/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    39649 2020-02-02 00:00:00.000000 catencfamily-0.0.75/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.75/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.75/README.md
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 catencfamily-0.0.75/pyproject.toml
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.75/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.76/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    87814 2020-02-02 00:00:00.000000 catencfamily-0.0.76/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    40405 2020-02-02 00:00:00.000000 catencfamily-0.0.76/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.76/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.76/README.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 catencfamily-0.0.76/pyproject.toml
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 catencfamily-0.0.76/PKG-INFO
```

### Comparing `catencfamily-0.0.75/src/catencfamily/encoders.py` & `catencfamily-0.0.76/src/catencfamily/encoders.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.75/src/catencfamily/utils.py` & `catencfamily-0.0.76/src/catencfamily/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -914,15 +914,17 @@
             );
     plt.title(title)
     
 
     
 # Community visualization
 # Kaggle: https://www.kaggle.com/code/rahulgoel1106/commmunity-detection-using-igraph-and-networkx
-def communityVisualization(filename, pathToFolder, algo = nx.community.greedy_modularity_communities , ax= None, title = None, withLabels = False, font_size = 8, edgewidth = 0.1, colorList =  ["orange", "yellow", "white"]):
+def communityVisualization(filename, pathToFolder, algo = nx.community.greedy_modularity_communities ,
+                           ax= None, title = None, withLabels = False, font_size = 8, edgewidth = 0.1,
+                           colorList =  ["orange","yellow","cyan","green","red"]):
     """
     Desc
     ----
     Displays communities created by given community algo.
 
     Parameters
     ----------
@@ -934,47 +936,55 @@
                     nx.community.greedy_modularity_communities
                     nx.community.louvain_communities
     ax: Matplotlib axis object
     withLabels : boolean, Should labels be displayed? The default is False.
     font_size : int, Label font size. The default is 8.
     edgewidth: float, Edge line width
     colorList: List of colors for difft communitied. 
-               Default is: ["orange", "yellow", "white"]
+               Default is: ["orange","yellow","cyan","green","red"]
 
     Returns
     -------
     None.
 
     """
     filepath = pathToFolder / filename
     G = nx.read_gml(filepath) 
     colors = colorList
     pos = nx.spring_layout(G)
-    lst_b = algo(G)
+    
+    if algo == nx.community.girvan_newman:
+        lst_b = algo(G)
+        lst_b = tuple(sorted(c) for c in next(lst_b))
+        lst_b = [frozenset(i) for i in lst_b ]
+    else:
+        lst_b = algo(G)
+
+    
     color_map_b = {}
     keys = G.nodes()
     values = "black"
     for i in keys:
             color_map_b[i] = values
     counter = 0
     for x in lst_b:
       for n in x:
-        color_map_b[n] = colors[counter]
+        color_map_b[n] = colorList[counter]
       counter = counter + 1
     nx.draw_networkx_edges(G, pos, width = edgewidth, ax =ax);
     nx.draw_networkx_nodes(G, pos, node_color=dict(color_map_b).values(), ax =ax);
     if withLabels:
       nx.draw_networkx_labels(G, pos, font_size = font_size, font_weight = 'bold',ax =ax)
     plt.axis("off");
     plt.title(title)
     #plt.show();    
 
 
 
-def transformBinnedDF2Communities(columnNames,pathToGraphFolder, train_binned, algo):
+def transformBinnedDF2Communities(columnNames,pathToGraphFolder, train_binned, algo=nx.community.greedy_modularity_communities):
     """
     Desc
     -----
     Replace every column in the binned the Dataframe as per network community
     Example binned/discrete dataframe:
             'a'     'b
             --      ---
@@ -1056,21 +1066,27 @@
       filepath = Path(pathToGraphFolder) / file
       # Read the file as a network
       G = nx.read_gml(filepath)
 
       # 2.2 Calculate community classes using algo
       #    cm_mod contains as many frozensets of nodes
       #    as there are communities:
-      cm_mod = algo(G)
+          
+      if algo == nx.community.girvan_newman:
+          cm_mod = algo(G)
+          cm_mod = tuple(sorted(c) for c in next(cm_mod))
+          cm_mod = [frozenset(i) for i in cm_mod ]
+      else:
+          cm_mod = algo(G)
 
       # 3.0 We now create dict corresponding to
       #     all communities in cm_mod
       #    Example:
       #                 frozenset1         frozenset2
-      #   cm_mod:      {'434', '435' },    {'23' , '78'}
+      #   cm_mod:     [{'434', '435' },    {'23' , '78'}]
       #   fset_dict  {'434': 0, '435' :0, '23' : 1, '78': 1}
 
       counter = 0  # Assigns values in dict
       fset_dict = {}  # Start with blank dict
       # For every frozenset
       for i in cm_mod:
         # If set i is not a frozenset, make it so
@@ -1167,21 +1183,27 @@
       filepath = Path(pathToGraphFolder) / file
       # Read the file as a network
       G = nx.read_gml(filepath)
 
       # 2.2 Calculate community classes using algo
       #    cm_mod contains as many frozensets of nodes
       #    as there are communities:
-      cm_mod = algo(G)
+          
+      if algo == nx.community.girvan_newman:
+          cm_mod = algo(G)
+          cm_mod = tuple(sorted(c) for c in next(cm_mod))
+          cm_mod = [frozenset(i) for i in cm_mod ]
+      else:
+          cm_mod = algo(G)
 
       # 3.0 We now create dict corresponding to
       #     all communities in cm_mod
       #    Example:
       #                 frozenset1         frozenset2
-      #   cm_mod:      {'434', '435' },    {'23' , '78'}
+      #   cm_mod:     [ {'434', '435' },    {'23' , '78'}]
       #   fset_dict  {'434': 0, '435' :0, '23' : 1, '78': 1}
 
       counter = 0  # Assigns values in dict
       fset_dict = {}  # Start with blank dict
       # For every frozenset
       for i in cm_mod:
         if not isinstance(i,frozenset):
```

### Comparing `catencfamily-0.0.75/LICENSE` & `catencfamily-0.0.76/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.75/README.md` & `catencfamily-0.0.76/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.75/pyproject.toml` & `catencfamily-0.0.76/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.75"
+version = "0.0.76"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -23,8 +23,8 @@
   "cdlib",
   "matplotlib",
   "seaborn",
   "pathlib",
   "scipy"
 ]
 [project.urls]
-"Homepage" = "https://github.com/harnalashok/CatEncodersFamily"
+"Homepage" = "https://github.com/harnalashok/CatEncodersFamily"
```

### Comparing `catencfamily-0.0.75/PKG-INFO` & `catencfamily-0.0.76/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.75
+Version: 0.0.76
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

