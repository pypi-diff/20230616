# Comparing `tmp/Slpapy-0.3.23.tar.gz` & `tmp/Slpapy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.3.23.tar", last modified: Wed May 24 03:10:56 2023, max compression
+gzip compressed data, was "Slpapy-0.4.0.tar", last modified: Fri Jun 16 07:12:06 2023, max compression
```

## Comparing `Slpapy-0.3.23.tar` & `Slpapy-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 03:10:56.647200 Slpapy-0.3.23/
--rw-rw-rw-   0        0        0      160 2023-05-24 03:10:56.647200 Slpapy-0.3.23/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-24 03:10:56.605311 Slpapy-0.3.23/Slpapy/
--rw-rw-rw-   0        0        0     4837 2023-05-22 12:08:25.000000 Slpapy-0.3.23/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     2658 2023-05-12 06:14:48.000000 Slpapy-0.3.23/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:10:56.644207 Slpapy-0.3.23/Slpapy/Spatial_map_pic/
--rw-rw-rw-   0        0        0      645 2023-05-24 03:09:49.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/Spatial_map.py
--rw-rw-rw-   0        0        0       52 2023-05-10 02:09:03.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/readwrite.py
--rw-rw-rw-   0        0        0    43450 2023-05-24 03:01:37.000000 Slpapy-0.3.23/Slpapy/Spatial_map_pic/scatterplots.py
--rw-rw-rw-   0        0        0      263 2023-05-10 02:17:27.000000 Slpapy-0.3.23/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     6754 2023-05-18 07:49:27.000000 Slpapy-0.3.23/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:10:56.616282 Slpapy-0.3.23/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      160 2023-05-24 03:10:56.000000 Slpapy-0.3.23/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2023-05-24 03:10:56.000000 Slpapy-0.3.23/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 03:10:56.000000 Slpapy-0.3.23/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-05-24 03:10:56.000000 Slpapy-0.3.23/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-24 03:10:56.000000 Slpapy-0.3.23/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 03:10:56.647200 Slpapy-0.3.23/setup.cfg
--rw-rw-rw-   0        0        0      512 2023-05-24 03:10:44.000000 Slpapy-0.3.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:12:06.222623 Slpapy-0.4.0/
+-rw-rw-rw-   0        0        0      159 2023-06-16 07:12:06.221625 Slpapy-0.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 07:12:06.129394 Slpapy-0.4.0/Slpapy/
+-rw-rw-rw-   0        0        0     3581 2023-06-16 07:08:20.000000 Slpapy-0.4.0/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     2658 2023-05-12 06:14:48.000000 Slpapy-0.4.0/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:12:06.216639 Slpapy-0.4.0/Slpapy/Spatial_map_pic/
+-rw-rw-rw-   0        0        0      645 2023-05-24 03:09:50.000000 Slpapy-0.4.0/Slpapy/Spatial_map_pic/Spatial_map.py
+-rw-rw-rw-   0        0        0       52 2023-05-10 02:09:04.000000 Slpapy-0.4.0/Slpapy/Spatial_map_pic/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:24.000000 Slpapy-0.4.0/Slpapy/Spatial_map_pic/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:24.000000 Slpapy-0.4.0/Slpapy/Spatial_map_pic/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:24.000000 Slpapy-0.4.0/Slpapy/Spatial_map_pic/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.4.0/Slpapy/Spatial_map_pic/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.4.0/Slpapy/Spatial_map_pic/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.4.0/Slpapy/Spatial_map_pic/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:24.000000 Slpapy-0.4.0/Slpapy/Spatial_map_pic/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.4.0/Slpapy/Spatial_map_pic/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:24.000000 Slpapy-0.4.0/Slpapy/Spatial_map_pic/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.4.0/Slpapy/Spatial_map_pic/readwrite.py
+-rw-rw-rw-   0        0        0    43450 2023-05-24 03:01:38.000000 Slpapy-0.4.0/Slpapy/Spatial_map_pic/scatterplots.py
+-rw-rw-rw-   0        0        0      263 2023-05-10 02:17:28.000000 Slpapy-0.4.0/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     6070 2023-06-16 07:05:44.000000 Slpapy-0.4.0/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-06-16 07:12:06.151335 Slpapy-0.4.0/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-06-16 07:12:05.000000 Slpapy-0.4.0/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-06-16 07:12:05.000000 Slpapy-0.4.0/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 07:12:05.000000 Slpapy-0.4.0/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-06-16 07:12:05.000000 Slpapy-0.4.0/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-16 07:12:05.000000 Slpapy-0.4.0/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 07:12:06.222623 Slpapy-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-06-16 07:11:44.000000 Slpapy-0.4.0/setup.py
```

### Comparing `Slpapy-0.3.23/Slpapy/Data_reconstruction.py` & `Slpapy-0.4.0/Slpapy/Data_reconstruction.py`

 * *Files 22% similar despite different names*

```diff
@@ -92,45 +92,15 @@
         adata = adata[:, adata.var['mask'] != True]
         del adata.var['mask']
 
 
     # 标注注释
     if annotation is not None:
         annotation = str(annotation)
-        liball = pd.read_csv(f'{annotation}', )
+        liball = pd.read_csv(f'{annotation}' )
         #填充liball中的空值为unknow
         liball = liball.fillna('unknow')
-        adata.var['m/zs'] = adata.var_names
-        for i in liball.index:
-            t = liball.loc[i, 'm/z']
-            t = round(t, 2)
-            for j in adata.var_names:
-                tt = adata.var.loc[j, 'm/z']
-                if round(tt, 2) == t:
-                    if liball.loc[i, 'Name'] != 'unknow':
-                        adata.var.loc[j, 'm/zs'] = liball.loc[i, 'Name']
-                    else:
-                        adata.var.loc[j, 'm/zs'] = liball.loc[i, 'Formula']
-                    break
+        adata,var_names = liball['Name']
 
-        adata.var_names = adata.var['m/zs']
-        print(adata.var)
-        del adata.var['m/zs']
-
-        # 合并重复的m/z
-        if isinstance(adata.X, csr_matrix):
-            adata.X = adata.X.toarray()
-
-        df = pd.DataFrame(adata.X, columns=adata.var_names)
-        var = adata.var
-        # Step 2: 合并重复的列（基因）
-        merged_df = df.groupby(df.columns, axis=1).sum()
-        merged_var = var.groupby(var.index, axis=0).sum()
-        # Step 3: 创建新的anndata对象，用合并后的数据更新adata
-        adata_new = ad.AnnData(X=merged_df.values, obs=adata.obs, var=pd.DataFrame(index=merged_df.columns))
-
-        adata_new.obs = adata.obs
-        adata_new.var = merged_var
-        adata = adata_new
     # 保存adata
     adata.write(f'{XY}' + ".h5ad")
     return adata
```

### Comparing `Slpapy-0.3.23/Slpapy/MZ_ppm_match.py` & `Slpapy-0.4.0/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.23/Slpapy/Spatial_map_pic/Spatial_map.py` & `Slpapy-0.4.0/Slpapy/Spatial_map_pic/Spatial_map.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.23/Slpapy/Spatial_map_pic/_compat.py` & `Slpapy-0.4.0/Slpapy/Spatial_map_pic/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.23/Slpapy/Spatial_map_pic/_docs.py` & `Slpapy-0.4.0/Slpapy/Spatial_map_pic/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.23/Slpapy/Spatial_map_pic/_rcmod.py` & `Slpapy-0.4.0/Slpapy/Spatial_map_pic/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.23/Slpapy/Spatial_map_pic/_settings.py` & `Slpapy-0.4.0/Slpapy/Spatial_map_pic/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.23/Slpapy/Spatial_map_pic/_utils.py` & `Slpapy-0.4.0/Slpapy/Spatial_map_pic/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.23/Slpapy/Spatial_map_pic/beats.py` & `Slpapy-0.4.0/Slpapy/Spatial_map_pic/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.23/Slpapy/Spatial_map_pic/is_constant.py` & `Slpapy-0.4.0/Slpapy/Spatial_map_pic/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.23/Slpapy/Spatial_map_pic/logging.py` & `Slpapy-0.4.0/Slpapy/Spatial_map_pic/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.23/Slpapy/Spatial_map_pic/palettes.py` & `Slpapy-0.4.0/Slpapy/Spatial_map_pic/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.23/Slpapy/Spatial_map_pic/readwrite.py` & `Slpapy-0.4.0/Slpapy/Spatial_map_pic/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.23/Slpapy/Spatial_map_pic/scatterplots.py` & `Slpapy-0.4.0/Slpapy/Spatial_map_pic/scatterplots.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.23/Slpapy/processing_analyze.py` & `Slpapy-0.4.0/Slpapy/processing_analyze.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,23 +25,14 @@
     adata.obs = t
     adata.obsm['X_spacial'] = np.array(adata.obs.loc[:, 'X':'Y'])
     print('Space integration complete')
     return adata
 
 
 def pp_analyze(adata, onlyhighly):
-    # 显示在所有细胞中在每个单细胞中产生最高计数分数的脂质
-    # sc.pl.highest_expr_genes(adata, n_top=20, save='_highest_expr_protein.png')
-    # 小提琴图：表达基因的数量，每个细胞包含的表达量，线粒体基因表达量的百分比。
-    adata.var['mt'] = adata.var_names.str.startswith('MT-')  # 将线粒体基因标记为 mt
-    sc.pp.calculate_qc_metrics(adata, qc_vars=['mt'], percent_top=None,
-                               log1p=False, inplace=True)
-    sc.pl.violin(adata, 'total_counts', jitter=0.4, multi_panel=True,
-                 save='_total_counts.png')
-    adata = adata[adata.obs['total_counts'] != 0, :]
     # 归一化，使得不同细胞样本间可比
     sc.pp.normalize_total(adata, target_sum=1e4)
     sc.pp.log1p(adata)
     # 存储数据
     adata.raw = adata
     # 选择高变异基因
     if onlyhighly == True:
```

### Comparing `Slpapy-0.3.23/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.4.0/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

