# Comparing `tmp/hnet-1.2.1.tar.gz` & `tmp/hnet-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hnet-1.2.1.tar", last modified: Fri Jun  9 15:56:23 2023, max compression
+gzip compressed data, was "hnet-1.2.2.tar", last modified: Fri Jun 16 18:08:16 2023, max compression
```

## Comparing `hnet-1.2.1.tar` & `hnet-1.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 15:56:23.409699 hnet-1.2.1/
--rw-rw-rw-   0        0        0    11557 2020-11-19 13:38:07.000000 hnet-1.2.1/LICENSE
--rw-rw-rw-   0        0        0      135 2020-11-19 13:38:07.000000 hnet-1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     9596 2023-06-09 15:56:23.409699 hnet-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     9038 2022-09-17 20:51:55.000000 hnet-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 15:56:23.392743 hnet-1.2.1/hnet/
--rw-rw-rw-   0        0        0     1967 2023-06-09 15:55:03.000000 hnet-1.2.1/hnet/__init__.py
--rw-rw-rw-   0        0        0     3510 2020-11-19 13:38:07.000000 hnet-1.2.1/hnet/adjmat_vec.py
--rw-rw-rw-   0        0        0    12158 2023-04-16 12:24:30.000000 hnet-1.2.1/hnet/examples.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:56:23.408701 hnet-1.2.1/hnet/gui/
--rw-rw-rw-   0        0        0        0 2020-11-19 13:38:07.000000 hnet-1.2.1/hnet/gui/__init__.py
--rw-rw-rw-   0        0        0    31911 2020-11-19 13:38:07.000000 hnet-1.2.1/hnet/gui/hnet_gui.py
--rw-rw-rw-   0        0        0    61970 2023-04-16 12:23:14.000000 hnet-1.2.1/hnet/hnet.py
--rw-rw-rw-   0        0        0    26820 2023-06-09 15:54:02.000000 hnet-1.2.1/hnet/hnstats.py
--rw-rw-rw-   0        0        0    17829 2021-05-23 17:59:59.000000 hnet-1.2.1/hnet/network.py
--rw-rw-rw-   0        0        0     1413 2021-05-19 09:47:36.000000 hnet-1.2.1/hnet/savefig.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:56:23.407704 hnet-1.2.1/hnet.egg-info/
--rw-rw-rw-   0        0        0     9596 2023-06-09 15:56:23.000000 hnet-1.2.1/hnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-06-09 15:56:23.000000 hnet-1.2.1/hnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 15:56:23.000000 hnet-1.2.1/hnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      150 2023-06-09 15:56:23.000000 hnet-1.2.1/hnet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-09 15:56:23.000000 hnet-1.2.1/hnet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 15:56:23.410705 hnet-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1500 2023-04-16 11:37:26.000000 hnet-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:08:16.366400 hnet-1.2.2/
+-rw-rw-rw-   0        0        0    11557 2020-11-19 13:38:07.000000 hnet-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0      135 2020-11-19 13:38:07.000000 hnet-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     9555 2023-06-16 18:08:16.366400 hnet-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9038 2022-09-17 20:51:55.000000 hnet-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 18:08:16.327546 hnet-1.2.2/hnet/
+-rw-rw-rw-   0        0        0     2015 2023-06-16 17:46:45.000000 hnet-1.2.2/hnet/__init__.py
+-rw-rw-rw-   0        0        0     3510 2020-11-19 13:38:07.000000 hnet-1.2.2/hnet/adjmat_vec.py
+-rw-rw-rw-   0        0        0    12294 2023-06-16 17:52:33.000000 hnet-1.2.2/hnet/examples.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:08:16.365405 hnet-1.2.2/hnet/gui/
+-rw-rw-rw-   0        0        0        0 2020-11-19 13:38:07.000000 hnet-1.2.2/hnet/gui/__init__.py
+-rw-rw-rw-   0        0        0    31911 2020-11-19 13:38:07.000000 hnet-1.2.2/hnet/gui/hnet_gui.py
+-rw-rw-rw-   0        0        0    58397 2023-06-16 17:55:31.000000 hnet-1.2.2/hnet/hnet.py
+-rw-rw-rw-   0        0        0    26820 2023-06-09 15:54:02.000000 hnet-1.2.2/hnet/hnstats.py
+-rw-rw-rw-   0        0        0    17794 2023-06-16 17:40:12.000000 hnet-1.2.2/hnet/network.py
+-rw-rw-rw-   0        0        0     1413 2021-05-19 09:47:36.000000 hnet-1.2.2/hnet/savefig.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:08:16.351441 hnet-1.2.2/hnet.egg-info/
+-rw-rw-rw-   0        0        0     9555 2023-06-16 18:08:16.000000 hnet-1.2.2/hnet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-06-16 18:08:16.000000 hnet-1.2.2/hnet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 18:08:16.000000 hnet-1.2.2/hnet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2023-06-16 18:08:16.000000 hnet-1.2.2/hnet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-16 18:08:16.000000 hnet-1.2.2/hnet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 18:08:16.366400 hnet-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1871 2023-06-16 17:49:32.000000 hnet-1.2.2/setup.py
```

### Comparing `hnet-1.2.1/LICENSE` & `hnet-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hnet-1.2.1/PKG-INFO` & `hnet-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: hnet
-Version: 1.2.1
+Version: 1.2.2
 Summary: Graphical Hypergeometric Networks
 Home-page: https://erdogant.github.io/hnet
+Download-URL: https://github.com/erdogant/hnet/archive/1.2.2.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/erdogant/hnet/archive/1.2.1.tar.gz
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -199,9 +197,7 @@
 * [Sphinx](https://erdogant.github.io/hnet)
 * [Github](https://github.com/erdogant/hnet)
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
-
-
```

### Comparing `hnet-1.2.1/README.md` & `hnet-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hnet-1.2.1/hnet/__init__.py` & `hnet-1.2.2/hnet/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from hnet.hnet import hnet
 
 from hnet.hnet import (
     enrichment,
     compare_networks,
     to_undirected,
-    import_example,
+    # import_example,
     )
 
 from hnet.adjmat_vec import (
     vec2adjmat,
     adjmat2vec,
     )
 
+from datazets import get as import_example
+
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.2.1'
+__version__ = '1.2.2'
 
 # module level doc-string
 __doc__ = """
 HNET - Graphical Hypergeometric networks.
 =====================================================================
 
 Creation of networks from datasets with mixed datatypes and with unknown function.
```

### Comparing `hnet-1.2.1/hnet/adjmat_vec.py` & `hnet-1.2.2/hnet/adjmat_vec.py`

 * *Files identical despite different names*

### Comparing `hnet-1.2.1/hnet/examples.py` & `hnet-1.2.2/hnet/examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # import hnet
 # print(dir(hnet))
 # print(hnet.__version__)
 
+# %% test examples
+
+from hnet import hnet
+hn = hnet()
+df = hn.import_example()
+
+import hnet
+df=hnet.import_example('titanic')
+
 # %%
 import numpy as np
 import pandas as pd
 
 
 # %% Titanic case
 from hnet import hnet
```

### Comparing `hnet-1.2.1/hnet/gui/hnet_gui.py` & `hnet-1.2.2/hnet/gui/hnet_gui.py`

 * *Files identical despite different names*

### Comparing `hnet-1.2.1/hnet/hnet.py` & `hnet-1.2.2/hnet/hnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Contact     : erdogant@gmail.com
 # github      : https://github.com/erdogant/hnet
 # Licence     : See licences
 # -------------------------------------------------
 
 # %% Libraries
 import matplotlib.pyplot as plt
-import requests
+# import requests
 from tqdm import tqdm
 import numpy as np
 import pandas as pd
 import os
 import networkx as nx
 from sklearn.preprocessing import MinMaxScaler, LabelEncoder
 from scipy.stats import combine_pvalues
@@ -22,24 +22,23 @@
 from hnet.savefig import savefig
 import pypickle
 import colourmap
 import df2onehot
 import imagesc
 from ismember import ismember
 import warnings
+import datazets as dz
 warnings.filterwarnings("ignore")
 label_encoder = LabelEncoder()
 
 
 # %% Association learning across all variables
 class hnet():
     """HNET - Graphical Hypergeometric networks.
 
-    Description
-    -----------
     This is the main function to detect significant edge probabilities between pairs of vertices (node-links) given the input DataFrame.
 
     A multi-step process is performed which consisting 5 steps.
         1. Pre-processing: Typing and One-hot Enconding. Each feature is set as being categoric, numeric or is excluded. The typing can be user-defined or automatically determined on conditions. Encoding of features in a one-hot dense array is done for the categoric terms. The one-hot dense array is subsequently used to create combinatory features using k combinations over n features (without replacement).
         2. Combinations: Make smart combinations between features because many mutual exclusive classes do exists.
         3. Hypergeometric test: The final dense array is used to assess significance with the categoric features.
         4. Wilcoxon Ranksum: To assess significance across the numeric features (Xnumeric) in relation to the dense array (Xcombination), the Mann-Whitney-U test is performed.
@@ -367,16 +366,14 @@
             labx = self.results['labx']
         return simmatP, simmatLogP, labx
 
     # Make network d3
     def d3heatmap(self, summarize=False, savepath=None, directed=True, threshold=None, white_list=None, black_list=None, min_edges=None, figsize=(700, 700), vmax=None, showfig=True, verbose=3):
         """Interactive heatmap creator.
 
-        Description
-        -----------
         This function creates a interactive and stand-alone heatmap that is build on d3 javascript.
         d3heatmap is integrated into hnet and uses the -log10(P-value) adjacency matrix.
         Each column and index name represents a node whereas values >0 in the matrix represents an edge.
         Node links are build from rows to columns. Building the edges from row to columns only matters in directed cases.
         The network nodes and edges are adjusted in weight based on hte -log10(P-value), and colors are based on the category names.
 
         Parameters
@@ -451,16 +448,14 @@
         results['clust_labx'] = labx
         return results
 
     # Make network d3
     def d3graph(self, summarize=False, node_size_limits=[6, 15], savepath=None, node_color=None, directed=True, threshold=None, white_list=None, black_list=None, min_edges=None, charge=500, figsize=(1500, 1500), showfig=True, elastic=False, verbose=3):
         """Interactive network creator.
 
-        Description
-        -----------
         This function creates a interactive and stand-alone network that is build on d3 javascript.
         d3graph is integrated into hnet and uses the -log10(P-value) adjacency matrix.
         Each column and index name represents a node whereas values >0 in the matrix represents an edge.
         Node links are build from rows to columns. Building the edges from row to columns only matters in directed cases.
         The network nodes and edges are adjusted in weight based on hte -log10(P-value), and colors are based on the category names.
 
         Parameters
@@ -566,16 +561,14 @@
         # Return
         return {'G': d3.D3graph.G, 'savepath': d3.D3graph.config['filepath'], 'labx': labx}
 
     # Make network plot
     def plot(self, summarize=False, scale=2, dist_between_nodes=0.4, node_size_limits=[25, 500], directed=True, node_color=None, savepath=None, figsize=[15, 10], pos=None, layout='fruchterman_reingold', dpi=250, threshold=None, white_list=None, black_list=None, min_edges=None, showfig=True, verbose=3):
         """Make plot static network plot of the model results.
 
-        Description
-        -----------
         The results of hnet can be vizualized in several manners, one of them is a static network plot.
 
         Parameters
         ----------
         self : Object
             The output of .association_learning()
         summarize : bool, (default: False)
@@ -730,22 +723,20 @@
                 savefig(fig, config['savepath'], dpi=config['dpi'], transp=True)
 
         # Return
         Gout = {}
         Gout['G'] = G
         Gout['labx'] = labx
         Gout['pos'] = pos
-        return(Gout)
+        return Gout
 
     # Make plot of the association_learning
     def heatmap(self, summarize=False, cluster=False, figsize=[15, 15], savepath=None, threshold=None, white_list=None, black_list=None, min_edges=None, verbose=3):
         """Plot static heatmap.
 
-        Description
-        -----------
         A heatmap can be of use when the results becomes too large to plot in a network.
 
         Parameters
         ----------
         self : Object
             The output of .association_learning()
         summarize : bool, (default: False)
@@ -808,16 +799,14 @@
         except:
             print('[hnet] >Error: Heatmap failed. Try cluster=False')
 
     # Extract combined rules from association_learning
     def combined_rules(self, simmatP=None, labx=None, verbose=3):
         """Association testing and combining Pvalues using fishers-method.
 
-        Description
-        -----------
         Multiple variables (antecedents) can be associated to a single variable (consequent).
         To test the significance of combined associations we used fishers-method. The strongest connection will be sorted on top.
 
         Parameters
         ----------
         simmatP : matrix
             simmilarity matrix
@@ -869,39 +858,41 @@
 
         # Keep only lines with pvalues
         df_rules.dropna(how='any', subset=['Pfisher'], inplace=True)
         # Sort
         df_rules.sort_values(by=['Pfisher'], ascending=True, inplace=True)
         df_rules.reset_index(inplace=True, drop=True)
         # Return
-        return(df_rules)
+        return df_rules
 
     def import_example(self, data='titanic', url=None, sep=',', verbose=3):
         """Import example dataset from github source.
 
-        Description
-        -----------
         Import one of the few datasets from github source or specify your own download url link.
 
         Parameters
         ----------
         data : str
-            Name of datasets: 'sprinkler', 'grocery', 'titanic', 'student', 'fifa', 'cancer', 'waterpump'
+            Example of a few datasets are:
+            Name of datasets: 'sprinkler', 'titanic', 'student', 'fifa', 'cancer', 'waterpump', 'retail'
         url : str
             url link to to dataset.
-        verbose : int, (default: 3)
-            Print message to screen.
 
         Returns
         -------
         pd.DataFrame()
             Dataset containing mixed features.
 
+        References
+        ----------
+            * https://github.com/erdogant/datazets
+
         """
-        return import_example(data=data, url=url, sep=sep, verbose=verbose)
+        return dz.get(data=data, url=url, sep=sep)
+        # return import_example(data=data, url=url, sep=sep, verbose=verbose)
 
     # Save model
     def save(self, filepath='hnet_model.pkl', overwrite=False, verbose=3):
         """Save learned model in pickle file.
 
         Parameters
         ----------
@@ -1017,16 +1008,14 @@
     return out
 
 
 # %% Compute fit
 def enrichment(df, y, y_min=None, alpha=0.05, multtest='holm', dtypes='pandas', specificity='medium', excl_background=None, verbose=3):
     """Enrichment analysis.
 
-    Description
-    -----------
     Compute enrichment between input dataset and response variable y. Length of dataframe and y must be equal.
     The input dataset is converted into a one-hot dense array based on automatic typing ``dtypes='pandas'`` or user defined dtypes.
 
     Parameters
     ----------
     df : DataFrame
         Input Dataframe.
@@ -1113,23 +1102,21 @@
     out = hnstats._multipletestcorrection(out, config['multtest'], verbose=config['verbose'])
     # Keep only significant ones
     out = hnstats._filter_significance(out, config['alpha'], multtest)
     # Make dataframe
     out = pd.DataFrame(out)
     # Return
     if config['verbose']>=3: print('[hnet] >Fin')
-    return(out)
+    return out
 
 
 # %% Make adjacency matrix symmetric with repect to the diagonal
 def to_undirected(adjmat, method='logp', verbose=3):
     """Make adjacency matrix symmetric.
 
-    Description
-    -----------
     The adjacency matrix resulting from hnet is not neccesarily symmetric due to the statistics being used.
     In some cases, a symmetric matrix can be usefull. This function makes sure that values above the diagonal are the same as below the diagonal.
     Values above and below the diagnal are combined using the max or min value.
 
     Parameters
     ----------
     adjmat : array
@@ -1172,23 +1159,21 @@
 
             adjmatS[i, j] = score
             adjmatS[j, i] = score
 
     # Make dataframe and return
     adjmatS=pd.DataFrame(index=index, data=adjmatS, columns=columns, dtype=float)
     # Return
-    return(adjmatS)
+    return adjmatS
 
 
 # %% Comparison of two networks
 def compare_networks(adjmat_true, adjmat_pred, pos=None, showfig=True, width=15, height=8, verbose=3):
     """Compare two adjacency matrices and plot the differences.
 
-    Description
-    -----------
     Comparison of two networks based on two adjacency matrices. Both matrices should be of equal size and of type pandas DataFrame.
     The columns and rows between both matrices are matched if not ordered similarly.
 
     Parameters
     ----------
     adjmat_true : pd.DataFrame()
         First array.
@@ -1222,15 +1207,15 @@
     scores, adjmat_diff = network.compare_networks(adjmat_true,
                                                    adjmat_pred,
                                                    pos=pos,
                                                    showfig=showfig,
                                                    width=width,
                                                    height=height,
                                                    verbose=verbose)
-    return(scores, adjmat_diff)
+    return scores, adjmat_diff
 
 
 # %% Do the math
 def _do_the_math(df, X_comb, dtypes, X_labx, simmatP, simmat_labx, i, specificity, y_min, verbose=3):
     count = 0
     # Get response variable to test association
     y = X_comb.iloc[:, i].values.astype(str)
@@ -1270,125 +1255,14 @@
 
     if verbose>=4: print('')
 
     # Return
     return out, simmatP, simmat_labx
 
 
-# %% Import example dataset from github.
-def import_example(data='titanic', url=None, sep=',', verbose=3):
-    """Import example dataset from github source.
-
-    Description
-    -----------
-    Import one of the few datasets from github source or specify your own download url link.
-
-    Parameters
-    ----------
-    data : str
-        * 'sprinkler'
-        * 'titanic'
-        * 'student'
-        * 'fifa'
-        * 'cancer'
-        * 'waterpump'
-        * 'retail'
-        * 'grocery'
-    url : str
-        url link to to dataset.
-
-    Returns
-    -------
-    pd.DataFrame()
-        Dataset containing mixed features.
-
-    """
-    from urllib.parse import urlparse
-
-    if url is None:
-        if data=='sprinkler':
-            url='https://erdogant.github.io/datasets/sprinkler.zip'
-        elif data=='titanic':
-            url='https://erdogant.github.io/datasets/titanic_train.zip'
-        elif data=='student':
-            url='https://erdogant.github.io/datasets/student_train.zip'
-        elif data=='cancer':
-            url='https://erdogant.github.io/datasets/cancer_dataset.zip'
-        elif data=='fifa':
-            url='https://erdogant.github.io/datasets/FIFA_2018.zip'
-        elif data=='waterpump':
-            url='https://erdogant.github.io/datasets/waterpump/waterpump_test.zip'
-        elif data=='retail':
-            url='https://erdogant.github.io/datasets/marketing_data_online_retail_small.zip'
-            sep=';'
-        elif data=='grocery':
-            url='https://erdogant.github.io/datasets/grocery_products_purchase.zip'
-            sep=';'
-    else:
-        data = wget.filename_from_url(url)
-
-    if url is None:
-        if verbose>=3: print('Nothing to download.')
-        return None
-
-    curpath = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
-    filename = os.path.basename(urlparse(url).path)
-    PATH_TO_DATA = os.path.join(curpath, filename)
-    if not os.path.isdir(curpath):
-        os.makedirs(curpath, exist_ok=True)
-
-    # Check file exists.
-    if not os.path.isfile(PATH_TO_DATA):
-        if verbose>=3: print('Downloading [%s] dataset from github source..' %(data))
-        wget.download(url, PATH_TO_DATA)
-
-    # Import local dataset
-    if verbose>=3: print('Import dataset [%s]' %(data))
-    df = pd.read_csv(PATH_TO_DATA, sep=sep)
-
-    # Transform data in case of grocery
-    if data=='grocery':
-        # Split the column by commas
-        df = df.iloc[:, 0].str.split(',', expand=True)
-        # Rename columns
-        df.columns = [f'Product {i+1}' for i in range(df.shape[1])]
-
-    # Return
-    return df
-
-
-# %% Retrieve files files.
-class wget:
-    """Retrieve file from url."""
-
-    def filename_from_url(url):
-        """Return filename."""
-        return os.path.basename(url)
-
-    def download(url, writepath):
-        """Download.
-
-        Parameters
-        ----------
-        url : str.
-            Internet source.
-        writepath : str.
-            Directory to write the file.
-
-        Returns
-        -------
-        None.
-
-        """
-        r = requests.get(url, stream=True)
-        with open(writepath, "wb") as fd:
-            for chunk in r.iter_content(chunk_size=1024):
-                fd.write(chunk)
-
-
 def _check_import_d3blocks(verbose=3):
     try:
         import d3blocks
         status = True
     except:
         if verbose>=3: print('Error: The library [d3blocks] is not installed by default. Try: <pip install d3blocks>')
         status = False
```

### Comparing `hnet-1.2.1/hnet/hnstats.py` & `hnet-1.2.2/hnet/hnstats.py`

 * *Files identical despite different names*

### Comparing `hnet-1.2.1/hnet/network.py` & `hnet-1.2.2/hnet/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 
 # %% Libraries
 import matplotlib.pyplot as plt
 import pandas as pd
 import numpy as np
 from community import community_louvain
 import networkx as nx
-from sklearn.preprocessing import minmax_scale
-from sklearn.preprocessing import MinMaxScaler 
+from sklearn.preprocessing import minmax_scale, MinMaxScaler
 import df2onehot
 from ismember import ismember
 import classeval as clf
 
 #%% Make graph from adjacency matrix
 def to_graph(adjmat, verbose=3):
     """Convert adjacency matrix to graph.
```

### Comparing `hnet-1.2.1/hnet/savefig.py` & `hnet-1.2.2/hnet/savefig.py`

 * *Files identical despite different names*

### Comparing `hnet-1.2.1/hnet.egg-info/PKG-INFO` & `hnet-1.2.2/hnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: hnet
-Version: 1.2.1
+Version: 1.2.2
 Summary: Graphical Hypergeometric Networks
 Home-page: https://erdogant.github.io/hnet
+Download-URL: https://github.com/erdogant/hnet/archive/1.2.2.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Download-URL: https://github.com/erdogant/hnet/archive/1.2.1.tar.gz
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -199,9 +197,7 @@
 * [Sphinx](https://erdogant.github.io/hnet)
 * [Github](https://github.com/erdogant/hnet)
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
-
-
```

### Comparing `hnet-1.2.1/setup.py` & `hnet-1.2.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,15 +9,30 @@
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # Setup ------------
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
-     install_requires=['requests', 'colourmap', 'pypickle', 'classeval', 'matplotlib','numpy','pandas','statsmodels','networkx','python-louvain','tqdm','scikit-learn','ismember','imagesc','df2onehot','fsspec'],
+     install_requires=['colourmap',
+                       'pypickle',
+                       'classeval',
+                       'matplotlib',
+                       'numpy',
+                       'pandas',
+                       'statsmodels',
+                       'networkx',
+                       'python-louvain',
+                       'tqdm',
+                       'scikit-learn',
+                       'ismember',
+                       'imagesc',
+                       'df2onehot',
+                       'fsspec',
+                       'datazets'],
      python_requires='>=3',
      name='hnet',
      version=new_version,
      author="Erdogan Taskesen",
      author_email="erdogant@gmail.com",
      description="Graphical Hypergeometric Networks",
      long_description=long_description,
```

