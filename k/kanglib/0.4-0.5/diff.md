# Comparing `tmp/kanglib-0.4.tar.gz` & `tmp/kanglib-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanglib-0.4.tar", last modified: Thu Jun 15 22:16:56 2023, max compression
+gzip compressed data, was "kanglib-0.5.tar", last modified: Thu Jun 15 22:26:53 2023, max compression
```

## Comparing `kanglib-0.4.tar` & `kanglib-0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 22:16:56.743924 kanglib-0.4/
--rw-r--r--   0 kang       (501) staff       (20)     1809 2023-06-15 22:16:56.743820 kanglib-0.4/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)     1531 2023-06-15 22:12:18.000000 kanglib-0.4/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 22:16:56.743120 kanglib-0.4/kanglib/
--rw-r--r--   0 kang       (501) staff       (20)      121 2023-06-15 15:35:23.000000 kanglib-0.4/kanglib/__init__.py
--rw-r--r--   0 kang       (501) staff       (20)      658 2023-06-15 22:09:31.000000 kanglib-0.4/kanglib/calculations.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 22:16:56.743691 kanglib-0.4/kanglib.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)     1809 2023-06-15 22:16:56.000000 kanglib-0.4/kanglib.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      186 2023-06-15 22:16:56.000000 kanglib-0.4/kanglib.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-15 22:16:56.000000 kanglib-0.4/kanglib.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)        8 2023-06-15 22:16:56.000000 kanglib-0.4/kanglib.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-15 22:16:56.743952 kanglib-0.4/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      595 2023-06-15 22:16:48.000000 kanglib-0.4/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 22:26:53.584132 kanglib-0.5/
+-rw-r--r--   0 kang       (501) staff       (20)     2751 2023-06-15 22:26:53.584024 kanglib-0.5/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)     2473 2023-06-15 22:26:49.000000 kanglib-0.5/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 22:26:53.583423 kanglib-0.5/kanglib/
+-rw-r--r--   0 kang       (501) staff       (20)      121 2023-06-15 15:35:23.000000 kanglib-0.5/kanglib/__init__.py
+-rw-r--r--   0 kang       (501) staff       (20)     1627 2023-06-15 22:26:15.000000 kanglib-0.5/kanglib/calculations.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-15 22:26:53.583900 kanglib-0.5/kanglib.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)     2751 2023-06-15 22:26:53.000000 kanglib-0.5/kanglib.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      186 2023-06-15 22:26:53.000000 kanglib-0.5/kanglib.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-15 22:26:53.000000 kanglib-0.5/kanglib.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)        8 2023-06-15 22:26:53.000000 kanglib-0.5/kanglib.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-15 22:26:53.584162 kanglib-0.5/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      595 2023-06-15 22:26:44.000000 kanglib-0.5/setup.py
```

### Comparing `kanglib-0.4/PKG-INFO` & `kanglib-0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kanglib
-Version: 0.4
+Version: 0.5
 Summary: Kang lib of Python package: calculate my math function
 Home-page: https://github.com/williampolicy/code_pypi
 Author: xiaowen kang
 Author-email: kangxiaowen@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
@@ -56,7 +56,52 @@
 
 ---
 
 python setup.py sdist bdist_wheel
 
 twine upload dist/*
 
+---
+## 使用示例
+
+下面是如何使用 `kanglib.calculate_weighted_value` 函数的示例：
+
+```python
+import pandas as pd
+import kanglib
+import matplotlib.pyplot as plt
+import numpy as np
+
+# 创建一个日期范围
+dates = pd.date_range(start='2022-01-01', periods=365*2)
+
+# 创建活动水平DataFrame
+activity_levels_df = pd.DataFrame({
+    'date': dates,
+    'activity_level': np.random.rand(len(dates))
+})
+
+# 创建权重DataFrame
+weights_df = pd.DataFrame({
+    'date': dates,
+    'weight': np.random.rand(len(dates))
+})
+
+# 合并这两个DataFrame
+df = pd.merge(activity_levels_df, weights_df, on='date')
+
+# 使用calculate_weighted_value函数
+df = kanglib.calculate_weighted_value(df, ['activity_level'], 'weight', 'result')
+
+# 打印DataFrame
+print(df)
+
+# 绘制结果
+plt.plot(df['date'], df['result'])
+plt.title('Weighted Activity Level over Time')
+plt.xlabel('Date')
+plt.ylabel('Weighted Activity Level')
+plt.show()
+
+
+```
+
```

### Comparing `kanglib-0.4/README.md` & `kanglib-0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -46,7 +46,52 @@
 
 ---
 
 python setup.py sdist bdist_wheel
 
 twine upload dist/*
 
+---
+## 使用示例
+
+下面是如何使用 `kanglib.calculate_weighted_value` 函数的示例：
+
+```python
+import pandas as pd
+import kanglib
+import matplotlib.pyplot as plt
+import numpy as np
+
+# 创建一个日期范围
+dates = pd.date_range(start='2022-01-01', periods=365*2)
+
+# 创建活动水平DataFrame
+activity_levels_df = pd.DataFrame({
+    'date': dates,
+    'activity_level': np.random.rand(len(dates))
+})
+
+# 创建权重DataFrame
+weights_df = pd.DataFrame({
+    'date': dates,
+    'weight': np.random.rand(len(dates))
+})
+
+# 合并这两个DataFrame
+df = pd.merge(activity_levels_df, weights_df, on='date')
+
+# 使用calculate_weighted_value函数
+df = kanglib.calculate_weighted_value(df, ['activity_level'], 'weight', 'result')
+
+# 打印DataFrame
+print(df)
+
+# 绘制结果
+plt.plot(df['date'], df['result'])
+plt.title('Weighted Activity Level over Time')
+plt.xlabel('Date')
+plt.ylabel('Weighted Activity Level')
+plt.show()
+
+
+```
+
```

### Comparing `kanglib-0.4/kanglib.egg-info/PKG-INFO` & `kanglib-0.5/kanglib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kanglib
-Version: 0.4
+Version: 0.5
 Summary: Kang lib of Python package: calculate my math function
 Home-page: https://github.com/williampolicy/code_pypi
 Author: xiaowen kang
 Author-email: kangxiaowen@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
@@ -56,7 +56,52 @@
 
 ---
 
 python setup.py sdist bdist_wheel
 
 twine upload dist/*
 
+---
+## 使用示例
+
+下面是如何使用 `kanglib.calculate_weighted_value` 函数的示例：
+
+```python
+import pandas as pd
+import kanglib
+import matplotlib.pyplot as plt
+import numpy as np
+
+# 创建一个日期范围
+dates = pd.date_range(start='2022-01-01', periods=365*2)
+
+# 创建活动水平DataFrame
+activity_levels_df = pd.DataFrame({
+    'date': dates,
+    'activity_level': np.random.rand(len(dates))
+})
+
+# 创建权重DataFrame
+weights_df = pd.DataFrame({
+    'date': dates,
+    'weight': np.random.rand(len(dates))
+})
+
+# 合并这两个DataFrame
+df = pd.merge(activity_levels_df, weights_df, on='date')
+
+# 使用calculate_weighted_value函数
+df = kanglib.calculate_weighted_value(df, ['activity_level'], 'weight', 'result')
+
+# 打印DataFrame
+print(df)
+
+# 绘制结果
+plt.plot(df['date'], df['result'])
+plt.title('Weighted Activity Level over Time')
+plt.xlabel('Date')
+plt.ylabel('Weighted Activity Level')
+plt.show()
+
+
+```
+
```

### Comparing `kanglib-0.4/setup.py` & `kanglib-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kanglib',
-    version='0.4',
+    version='0.5',
     packages=find_packages(),
     description='Kang lib of Python package: calculate my math function',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',  # 添加这一行
     url='https://github.com/williampolicy/code_pypi',
     author='xiaowen kang',
     author_email='kangxiaowen@gmail.com',
```

