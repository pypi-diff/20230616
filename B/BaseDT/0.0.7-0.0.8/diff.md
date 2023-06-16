# Comparing `tmp/BaseDT-0.0.7.tar.gz` & `tmp/BaseDT-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseDT-0.0.7.tar", last modified: Fri Jun  9 06:53:39 2023, max compression
+gzip compressed data, was "dist/BaseDT-0.0.8.tar", last modified: Fri Jun 16 06:29:18 2023, max compression
```

## Comparing `BaseDT-0.0.7.tar` & `BaseDT-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-09 06:53:39.000000 BaseDT-0.0.7/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-09 06:53:39.000000 BaseDT-0.0.7/BaseDT/
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-04-26 07:17:02.000000 BaseDT-0.0.7/BaseDT/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)    31622 2023-06-07 06:26:00.000000 BaseDT-0.0.7/BaseDT/data.py
--rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-04-26 07:17:02.000000 BaseDT-0.0.7/BaseDT/data_image.py
--rw-rw-r--   0 user      (1001) user      (1001)    37221 2023-06-09 06:53:01.000000 BaseDT-0.0.7/BaseDT/dataset.py
--rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-04-26 07:17:02.000000 BaseDT-0.0.7/BaseDT/io.py
--rw-rw-r--   0 user      (1001) user      (1001)    12752 2023-06-06 05:32:46.000000 BaseDT-0.0.7/BaseDT/plot.py
--rw-rw-r--   0 user      (1001) user      (1001)     7577 2023-06-05 14:43:34.000000 BaseDT-0.0.7/BaseDT/utils.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-09 06:53:39.000000 BaseDT-0.0.7/BaseDT.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-09 06:53:39.000000 BaseDT-0.0.7/BaseDT.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      332 2023-06-09 06:53:39.000000 BaseDT-0.0.7/BaseDT.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-09 06:53:39.000000 BaseDT-0.0.7/BaseDT.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       43 2023-06-09 06:53:39.000000 BaseDT-0.0.7/BaseDT.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-06-09 06:53:39.000000 BaseDT-0.0.7/BaseDT.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-02-02 07:26:47.000000 BaseDT-0.0.7/BaseDT.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDT-0.0.7/MANIFEST.in
--rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-09 06:53:39.000000 BaseDT-0.0.7/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       42 2023-05-31 10:06:54.000000 BaseDT-0.0.7/install_requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-09 06:53:39.000000 BaseDT-0.0.7/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     4245 2023-06-09 06:53:21.000000 BaseDT-0.0.7/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-16 06:29:18.000000 BaseDT-0.0.8/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-16 06:29:18.000000 BaseDT-0.0.8/BaseDT/
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2023-04-26 07:17:02.000000 BaseDT-0.0.8/BaseDT/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)    31622 2023-06-07 06:26:00.000000 BaseDT-0.0.8/BaseDT/data.py
+-rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-04-26 07:17:02.000000 BaseDT-0.0.8/BaseDT/data_image.py
+-rw-rw-r--   0 user      (1001) user      (1001)    37236 2023-06-09 06:59:00.000000 BaseDT-0.0.8/BaseDT/dataset.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-04-26 07:17:02.000000 BaseDT-0.0.8/BaseDT/io.py
+-rw-rw-r--   0 user      (1001) user      (1001)    13050 2023-06-16 06:28:08.000000 BaseDT-0.0.8/BaseDT/plot.py
+-rw-rw-r--   0 user      (1001) user      (1001)     7577 2023-06-05 14:43:34.000000 BaseDT-0.0.8/BaseDT/utils.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-06-16 06:29:18.000000 BaseDT-0.0.8/BaseDT.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-16 06:29:18.000000 BaseDT-0.0.8/BaseDT.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      332 2023-06-16 06:29:18.000000 BaseDT-0.0.8/BaseDT.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-06-16 06:29:18.000000 BaseDT-0.0.8/BaseDT.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       43 2023-06-16 06:29:18.000000 BaseDT-0.0.8/BaseDT.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-06-16 06:29:18.000000 BaseDT-0.0.8/BaseDT.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-02-02 07:26:47.000000 BaseDT-0.0.8/BaseDT.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDT-0.0.8/MANIFEST.in
+-rw-rw-r--   0 user      (1001) user      (1001)      314 2023-06-16 06:29:18.000000 BaseDT-0.0.8/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       42 2023-05-31 10:06:54.000000 BaseDT-0.0.8/install_requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-06-16 06:29:18.000000 BaseDT-0.0.8/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     4245 2023-06-16 06:28:25.000000 BaseDT-0.0.8/setup.py
```

### Comparing `BaseDT-0.0.7/BaseDT/data.py` & `BaseDT-0.0.8/BaseDT/data.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.7/BaseDT/data_image.py` & `BaseDT-0.0.8/BaseDT/data_image.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.7/BaseDT/dataset.py` & `BaseDT-0.0.8/BaseDT/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -873,10 +873,10 @@
     np.savetxt(train_file, train_data_with_header, delimiter=",", fmt="%s")
     np.savetxt(val_file, val_data_with_header, delimiter=",", fmt="%s")
 
     return train_x,train_y, val_x, val_y
 
 if __name__=="__main__":
     path = "../iris/iris.csv"
-    train_x,train_y,val_x,val_y = split_tab_dataset(path,data_column=range(0,4),label_column=4)
+    train_x,train_y,val_x,val_y = split_tab_dataset(path,data_column=range(0,4),label_column=4,normalize=True)
```

### Comparing `BaseDT-0.0.7/BaseDT/io.py` & `BaseDT-0.0.8/BaseDT/io.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.7/BaseDT/plot.py` & `BaseDT-0.0.8/BaseDT/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,17 +242,20 @@
     'bbox': dict(facecolor='black', alpha=0.5, boxstyle='Round'),
     'verticalalignment': 'top',
     'horizontalalignment': 'left',
 }
 def draw_single_cls(image, result):
     texts = []
     max_length = 12 # 文本长度限制
-    texts.append('Pred_label: {}'.format(result['标签']))
-    texts.append('Pred_score: {:.2f}'.format(result['置信度']))
-    texts.append('Pred_label: {}'.format(result['预测结果'][:max_length]))
+    if '标签' in result:
+        texts.append('Pred_label: {}'.format(result['标签']))
+    if '置信度' in result:
+        texts.append('Pred_score: {:.2f}'.format(result['置信度']))
+    if '预测结果' in result:
+        texts.append('Pred_label: {}'.format(result['预测结果'][:max_length]))
     text = '\n'.join(texts)
     #fig = plt.figure()
     image.init_plt()
     img_tmp = image._image
     img_scale = get_adaptive_scale(img_tmp.shape[:2])
     DEFAULT_TEXT_CFG['size'] = int(img_scale * 5)
     pos = np.array([[img_scale*5, img_scale*5]], dtype=int)
@@ -304,29 +307,33 @@
     assert len(dataset_palette) >= num_classes, \
         'The length of palette should not be less than `num_classes`.'
     return dataset_palette
 
 def draw_single_det(image, result, line_width: int =3) -> None:
     assert isinstance(result, list), "Expected 'result' to be a list"
     image.init_plt()
+    if len(result) == 0:
+        return
     bboxes = []
     labels = []
     label_texts = []
     for bbox in result:
         assert isinstance(bbox, dict), "Expected each element in 'result' to be a dictionary"
         assert '坐标' in bbox and '标签' in bbox, "Each dictionary in 'result' should have '坐标' and '标签' keys"
         
         coords = bbox['坐标']
         assert isinstance(coords, dict), "Expected '坐标' to be a dictionary"
         assert all(key in coords for key in ['x1', 'y1', 'x2', 'y2']), "The '坐标' dictionary should have 'x1', 'y1', 'x2', 'y2' keys"
         
         bboxes.append([coords['x1'], coords['y1'], coords['x2'], coords['y2']])
         labels.append(bbox['标签'])
-        label_texts.append('{}:{}'.format(bbox['预测结果'],round(float(bbox['置信度']) * 100, 1)))
-
+        if '预测结果' in bbox:
+            label_texts.append('{}:{}'.format(bbox['预测结果'],round(float(bbox['置信度']) * 100, 1)))
+        else:
+            label_texts.append('{}:{}'.format(bbox['标签'],round(float(bbox['置信度']) * 100, 1)))
     bboxes = np.array(bboxes)
     labels = np.array(labels)
 
 
     max_label = int(max(labels) if len(labels) > 0 else 0)
 
     bbox_palette = get_palette(max_label + 1)
```

### Comparing `BaseDT-0.0.7/BaseDT/utils.py` & `BaseDT-0.0.8/BaseDT/utils.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.7/setup.py` & `BaseDT-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 yield item
 
     packages = list(gen_packages_items())
     return packages
 
 setup(
     name='BaseDT',
-    version='0.0.7',
+    version='0.0.8',
     # version='0.0.1rc1',
     description='BaseDT is a data-processing  tool including data, dataset, io and plot.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
```

