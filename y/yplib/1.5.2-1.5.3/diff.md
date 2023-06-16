# Comparing `tmp/yplib-1.5.2.tar.gz` & `tmp/yplib-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.5.2.tar", last modified: Fri Jun 16 06:49:21 2023, max compression
+gzip compressed data, was "dist\yplib-1.5.3.tar", last modified: Fri Jun 16 08:09:06 2023, max compression
```

## Comparing `yplib-1.5.2.tar` & `yplib-1.5.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 06:49:21.888373 yplib-1.5.2/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.5.2/LICENSE
--rw-rw-rw-   0        0        0      352 2023-06-16 06:49:21.888199 yplib-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.5.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 06:49:21.888833 yplib-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-06-16 06:49:18.000000 yplib-1.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:49:21.885251 yplib-1.5.2/yplib/
--rw-rw-rw-   0        0        0      357 2023-06-16 03:11:06.000000 yplib-1.5.2/yplib/__init__.py
--rw-rw-rw-   0        0        0    11382 2023-06-16 02:00:45.000000 yplib-1.5.2/yplib/chart.py
--rw-rw-rw-   0        0        0     8021 2023-06-16 00:23:59.000000 yplib-1.5.2/yplib/chart_html.py
--rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.5.2/yplib/file.py
--rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.5.2/yplib/html_parser.py
--rw-rw-rw-   0        0        0    21122 2023-06-16 06:49:01.000000 yplib-1.5.2/yplib/index.py
-drwxrwxrwx   0        0        0        0 2023-06-16 06:49:21.887204 yplib-1.5.2/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-06-16 06:49:21.000000 yplib-1.5.2/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-16 06:49:21.000000 yplib-1.5.2/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 06:49:21.000000 yplib-1.5.2/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 06:49:21.000000 yplib-1.5.2/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 08:09:06.304903 yplib-1.5.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.5.3/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-06-16 08:09:06.304568 yplib-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-1.5.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 08:09:06.304903 yplib-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-06-16 08:08:49.000000 yplib-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:09:06.300415 yplib-1.5.3/yplib/
+-rw-rw-rw-   0        0        0      357 2023-06-16 03:11:06.000000 yplib-1.5.3/yplib/__init__.py
+-rw-rw-rw-   0        0        0    11382 2023-06-16 02:00:45.000000 yplib-1.5.3/yplib/chart.py
+-rw-rw-rw-   0        0        0     8228 2023-06-16 08:08:13.000000 yplib-1.5.3/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     6984 2023-06-16 00:59:15.000000 yplib-1.5.3/yplib/file.py
+-rw-rw-rw-   0        0        0      829 2023-06-16 03:07:17.000000 yplib-1.5.3/yplib/html_parser.py
+-rw-rw-rw-   0        0        0    21122 2023-06-16 06:49:01.000000 yplib-1.5.3/yplib/index.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:09:06.303898 yplib-1.5.3/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-06-16 08:09:06.000000 yplib-1.5.3/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-16 08:09:06.000000 yplib-1.5.3/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 08:09:06.000000 yplib-1.5.3/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 08:09:06.000000 yplib-1.5.3/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.5.2/LICENSE` & `yplib-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.5.2/setup.py` & `yplib-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.5.2",
+  version="1.5.3",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-1.5.2/yplib/chart.py` & `yplib-1.5.3/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.2/yplib/chart_html.py` & `yplib-1.5.3/yplib/chart_html.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,15 +50,15 @@
              '        left: "30px",' \
              '        right: "40px",' \
              '        bottom: "80px",' \
              '        containLabel: true,' \
              '    },' \
              '    toolbox: {' \
              '        feature: {' \
-             '            saveAsImage: {},' \
+             '            saveAsImage: {pixelRatio:5},' \
              '        },' \
              '    },' \
              '    yAxis: {' \
              '        type: "value",' \
              '    },' \
              '    xAxis: {' \
              '        type: "category",' \
@@ -80,15 +80,15 @@
              '    trigger: "axis",' \
              '  },' \
              '  title: {' \
              '    text: "-chart_name-"' \
              '  },' \
              '  toolbox: {' \
              '    feature: {' \
-             '      saveAsImage: {}' \
+             '      saveAsImage: {pixelRatio:5}' \
              '    }' \
              '  },' \
              '    grid: {' \
              '        left: "30px",' \
              '        right: "40px",' \
              '        bottom: "80px",' \
              '        containLabel: true,' \
@@ -145,14 +145,19 @@
              '  title: {' \
              '    text: "-chart_name-",' \
              '    left: 10' \
              '  },' \
              '  tooltip: {' \
              '    trigger: "item"' \
              '  },' \
+             '    toolbox: {' \
+             '        feature: {' \
+             '            saveAsImage: {pixelRatio:5},' \
+             '        },' \
+             '    },' \
              '  legend: {' \
              '    top: "5%",' \
              '    left: "center"' \
              '  },' \
              '  series: [' \
              '    {' \
              '      name: "-chart_name-",' \
@@ -189,15 +194,15 @@
              '  },' \
              '  toolbox: {' \
              '    feature: {' \
              '      dataZoom: {' \
              '        yAxisIndex: false' \
              '      },' \
              '      saveAsImage: {' \
-             '        pixelRatio: 2' \
+             '        pixelRatio: 5' \
              '      }' \
              '    }' \
              '  },' \
              '  tooltip: {' \
              '    trigger: "axis",' \
              '    axisPointer: {' \
              '      type: "shadow"' \
```

### Comparing `yplib-1.5.2/yplib/file.py` & `yplib-1.5.3/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.2/yplib/html_parser.py` & `yplib-1.5.3/yplib/html_parser.py`

 * *Files identical despite different names*

### Comparing `yplib-1.5.2/yplib/index.py` & `yplib-1.5.3/yplib/index.py`

 * *Files identical despite different names*

