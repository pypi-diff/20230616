# Comparing `tmp/tkintertools-2.6.4.tar.gz` & `tmp/tkintertools-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-2.6.4.tar", last modified: Mon Jun 12 07:46:34 2023, max compression
+gzip compressed data, was "tkintertools-2.6.5.tar", last modified: Fri Jun 16 17:36:10 2023, max compression
```

## Comparing `tkintertools-2.6.4.tar` & `tkintertools-2.6.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 07:46:34.462242 tkintertools-2.6.4/
--rw-rw-rw-   0        0        0     7548 2023-06-12 04:45:59.000000 tkintertools-2.6.4/LICENSE
--rw-rw-rw-   0        0        0    28785 2023-06-12 07:46:34.461238 tkintertools-2.6.4/PKG-INFO
--rw-rw-rw-   0        0        0    28224 2023-06-12 07:44:21.000000 tkintertools-2.6.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 07:46:34.462242 tkintertools-2.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1290 2023-06-12 03:22:11.000000 tkintertools-2.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:46:34.450724 tkintertools-2.6.4/tkintertools/
--rw-rw-rw-   0        0        0     2336 2023-06-12 07:17:43.000000 tkintertools-2.6.4/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    62557 2023-06-10 12:15:00.000000 tkintertools-2.6.4/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     2066 2023-06-10 13:59:58.000000 tkintertools-2.6.4/tkintertools/constants.py
--rw-rw-rw-   0        0        0    18169 2023-06-12 04:42:07.000000 tkintertools-2.6.4/tkintertools/tools_3d.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:46:34.459819 tkintertools-2.6.4/tkintertools.egg-info/
--rw-rw-rw-   0        0        0    28785 2023-06-12 07:46:34.000000 tkintertools-2.6.4/tkintertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-06-12 07:46:34.000000 tkintertools-2.6.4/tkintertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 07:46:34.000000 tkintertools-2.6.4/tkintertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-12 07:46:34.000000 tkintertools-2.6.4/tkintertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 17:36:10.472603 tkintertools-2.6.5/
+-rw-rw-rw-   0        0        0     9257 2023-06-12 07:55:24.000000 tkintertools-2.6.5/LICENSE.txt
+-rw-rw-rw-   0        0        0    28817 2023-06-16 17:36:10.470597 tkintertools-2.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0    28252 2023-06-16 17:34:58.000000 tkintertools-2.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 17:36:10.472603 tkintertools-2.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-06-16 17:04:04.000000 tkintertools-2.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:36:10.460519 tkintertools-2.6.5/tkintertools/
+-rw-rw-rw-   0        0        0     2859 2023-06-16 17:07:18.000000 tkintertools-2.6.5/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    62351 2023-06-16 16:33:00.000000 tkintertools-2.6.5/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     1999 2023-06-16 16:48:27.000000 tkintertools-2.6.5/tkintertools/constants.py
+-rw-rw-rw-   0        0        0    21400 2023-06-16 17:26:13.000000 tkintertools-2.6.5/tkintertools/tools_3d.py
+drwxrwxrwx   0        0        0        0 2023-06-16 17:36:10.467935 tkintertools-2.6.5/tkintertools.egg-info/
+-rw-rw-rw-   0        0        0    28817 2023-06-16 17:36:10.000000 tkintertools-2.6.5/tkintertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-06-16 17:36:10.000000 tkintertools-2.6.5/tkintertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 17:36:10.000000 tkintertools-2.6.5/tkintertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-16 17:36:10.000000 tkintertools-2.6.5/tkintertools.egg-info/top_level.txt
```

### Comparing `tkintertools-2.6.4/LICENSE` & `tkintertools-2.6.5/LICENSE.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-木兰宽松许可证, 第2版
+木兰宽松许可证, 第2版 木兰宽松许可证， 第2版
 
 2020年1月 http://license.coscl.org.cn/MulanPSL2
 
 您对"软件"的复制、使用、修改及分发受木兰宽松许可证，第2版（"本许可证"）的如下条款的约束：
 
    0. 定义
 
@@ -38,15 +38,45 @@
 
    6. 语言
 
    "本许可证"以中英文双语表述，中英文版本具有同等法律效力。如果中英文版本存在任何冲突不一致，以中文版为准。
 
 条款结束
 
-Mulan Permissive Software License，Version 2 (Mulan PSL v2)
+如何将木兰宽松许可证，第2版，应用到您的软件
+
+如果您希望将木兰宽松许可证，第2版，应用到您的新软件，为了方便接收者查阅，建议您完成如下三步：
+
+   1， 请您补充如下声明中的空白，包括软件名、软件的首次发表年份以及您作为版权人的名字；
+
+   2， 请您在软件包的一级目录下创建以"LICENSE"为名的文件，将整个许可证文本放入该文件中；
+
+   3， 请将如下声明文本放入每个源文件的头部注释中。
+
+Copyright (c) 2022 小康2022
+
+tkintertools is licensed under Mulan PSL v2.
+
+You can use this software according to the terms and conditions of the Mulan PSL v2.
+
+You may obtain a copy of Mulan PSL v2 at:
+
+http://license.coscl.org.cn/MulanPSL2
+
+THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND,
+
+EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT,
+
+MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.
+
+See the Mulan PSL v2 for more details.
+
+
+
+Mulan Permissive Software License，Version 2 Mulan Permissive Software License，Version 2 (Mulan PSL v2)
 
 January 2020 http://license.coscl.org.cn/MulanPSL2
 
 Your reproduction, use, modification and distribution of the Software shall be subject to Mulan PSL v2 (this License) with the following terms and conditions:
 
    0. Definition
 
@@ -82,26 +112,34 @@
 
    6. Language
 
    THIS LICENSE IS WRITTEN IN BOTH CHINESE AND ENGLISH, AND THE CHINESE VERSION AND ENGLISH VERSION SHALL HAVE THE SAME LEGAL EFFECT. IN THE CASE OF DIVERGENCE BETWEEN THE CHINESE AND ENGLISH VERSIONS, THE CHINESE VERSION SHALL PREVAIL.
 
 END OF THE TERMS AND CONDITIONS
 
-=======================================================================================
+How to Apply the Mulan Permissive Software License，Version 2 (Mulan PSL v2) to Your Software
+
+To apply the Mulan PSL v2 to your work, for easy identification by recipients, you are suggested to complete following three steps:
+
+   i. Fill in the blanks in following statement, including insert your software name, the year of the first publication of your software, and your name identified as the copyright owner;
+
+   ii. Create a file named "LICENSE" which contains the whole context of this License in the first directory of your software package;
+
+   iii. Attach the statement to the appropriate annotated syntax at the beginning of each source file.
 
-Copyright (c) 2022-2023 小康2022
+Copyright (c) 2022 Xiaokang2022
 
-[tkintertools] is licensed under Mulan PSL v2.
+tkintertools is licensed under Mulan PSL v2.
 
 You can use this software according to the terms and conditions of the Mulan PSL v2.
 
 You may obtain a copy of Mulan PSL v2 at:
 
 http://license.coscl.org.cn/MulanPSL2
 
 THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND,
 
 EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT,
 
 MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.
 
-See the Mulan PSL v2 for more details. 
+See the Mulan PSL v2 for more details.
```

### Comparing `tkintertools-2.6.4/PKG-INFO` & `tkintertools-2.6.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,203 +1,180 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.4
-Summary: An auxiliary module of the tkinder module
+Version: 2.6.5
+Summary: An auxiliary module of the tkinter module
 Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 License: MulanPSL-2.0
 Keywords: tkinter,tkintertools,GUI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.txt
 
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
-    <p><img height="120px" alt="logo.png" src="tkintertools.png" /></p>
+    <p><img height="128px" alt="logo.png" src="tkt.png" /></p>
     <p>
     The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module
     <br />
     <code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块
     </p>
     <p>
-        <a href="tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.4-blue" alt="latest version" />
+        <a href="https://github.com/Xiaokang2022/tkintertools">
+            <img src="https://img.shields.io/badge/Version-2.6.5-blue" alt="latest version" />
         </a>
-        <a href="LICENSE">
+        <a href="LICENSE.txt">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
         <a href="CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/06/12-orange" alt="ChangeLog" />
+            <img src="https://img.shields.io/badge/ChangeLog-2023/06/17-orange" alt="ChangeLog" />
         </a>
         <a href="TODO.md">
-            <img src="https://img.shields.io/badge/ToDo-15-yellow?logo=cachet" alt="ToDos" />
+            <img src="https://img.shields.io/badge/ToDo-14-yellow?logo=cachet" alt="ToDo" />
         </a>
-        <a href="https://pypistats.org/packages/tkintertools">
-            <img src="https://img.shields.io/badge/Download-4k-purple?logo=pypi" alt="Downloads" />
+        <a href="https://github.com/Xiaokang2022/tkintertools/wiki">
+            <img src="https://img.shields.io/badge/Wiki-15-purple" alt="Wiki" />
         </a>
         <br />
-        <a href="mailto:2951256653@qq.com">
-            <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
+        <a href="https://pypistats.org/packages/tkintertools">
+            <img src="https://img.shields.io/badge/Download-6k-white?logo=pypi" alt="Downloads" />
         </a>
         <a href="https://github.com/Xiaokang2022">
-            <img src="https://img.shields.io/badge/Author-小康2022-white" alt="Author" />
+            <img src="https://img.shields.io/badge/Author-小康2022-springgreen" alt="Author" />
         </a>
         <a href="https://xiaokang2022.blog.csdn.net">
             <img src="https://img.shields.io/badge/Blog-小康2022@CSDN-red" alt="Blog" />
         </a>
+        <a href="mailto:2951256653@qq.com">
+            <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
+        </a>
     </p>
 </div>
 
-Installation/模块安装
---------------------
+Install/模块安装
+---------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.4
-* Release Date/发布日期 : 2023/06/12
+* Version/版本 : `2.6.5`
+* Release Date/发布日期 : 2023/06/17 (UTC+08)
 
-这个是目前的最新稳定版，比较稳定，bug （可能）没有那么多，推荐使用这个。  
-关于稳定版有 Issue 的话，我会去查看并尝试解决 Issue。
+这个是目前的最新稳定版，比较稳定，bug（可能）没有那么多，推荐使用这个。  
+稳定版 bug 不一定少，但它至少是我在多个操作系统中测试过的，是跨平台的，兼容的。
 
 ```
-pip install tkintertools==2.6.4
+pip install tkintertools==2.6.5
 ```
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.4
-* Release Date/发布日期 : 2023/06/11
+* Version/版本 : `2.6.5`
+* Release Date/发布日期 : 2023/06/13 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 也可能会比较多，但也可能会比原来的版本更加稳定。  
-大家可以在 Issue 中提出一些建议，我会适当采纳一些并在开发版本中更改或实现。
+开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。  
+大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 ```
-pip install tkintertools-dev==2.6.4
+pip install tkintertools-dev==2.6.5
 ```
 
-**特别注意**
-* 开发版仅作示例，各函数或类的API并非最终确定结果，直接使用开发版可能导致后续无法与正式版兼容！
-* 若要使用开发版，请先卸载正式版后再进行pip安装，再次使用正式版时也是一样，先卸载开发版再安装正式版！
+**Attention/特别注意**
+* 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！
+* 若要使用开发版，请先卸载稳定版后再进行 pip 安装，再次使用稳定版时也是一样，先卸载开发版再安装稳定版！
 
 ### Environmental requirements/环境需求
 
-没有任何额外的依赖包（除了tkinter），但只支持以下 Python 版本:
+没有任何额外的依赖包（除了 tkinter），但只支持以下 Python 版本:
 
 ![Python3.8](https://img.shields.io/badge/Python-3.8.*-blue?logo=python)
 ![Python3.9](https://img.shields.io/badge/Python-3.9.*-blue?logo=python)
 ![Python3.10](https://img.shields.io/badge/Python-3.10.*-blue?logo=python)
 ![Python3.11](https://img.shields.io/badge/Python-3.11.*-blue?logo=python)
 ![Python3.12](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 可能在某些操作系统上也可运行，但目前以下操作系统已经测试通过:
 
 ![Windows10](https://img.shields.io/badge/Windows-10-green?logo=windows)
 ![Windows11](https://img.shields.io/badge/Windows-11-green?logo=windows11)
 ![Ubuntu22.04](https://img.shields.io/badge/Ubuntu-22.04-green?logo=ubuntu)
 
-<a name="news">News/最新功能</a>
+News/最新功能
 ------------
 
-最新版的 tkintertools **开发版**(2.6.4-dev)新增了对3d几何体空间位置排序的支持，使得几何体不再只有粗略的线条，而拥有丰富的颜色。
+**最新版本: tkintertools-2.6.5 稳定版**
 
-在 Windows 系统下运行下面的示例程序时，其拥有以下功能：
+**【重磅炸裂更新：新增了 Wiki 供大家查看，方便大家迅速掌握 tkintertools 的使用方法和小技巧！[点此传送](https://github.com/Xiaokang2022/tkintertools/wiki)】**
+
+    【特别说明】
+    近期本人将暂时停止对 tkintertools 模块本身的更新，本人先去完善 Wiki 再继续更新 tkintertools！
+    此外，README.md 中关于模块内容详细介绍的部分将逐步转移到 Wiki 中！
+
+下面是本次版本更新内容条目：
+
+- [X] 子模块 `tools_3d` 新增类 `Space` 可以直接提供对 3D 对象进行平移、旋转和缩放等操作的功能
+- [X] 修复了类 `Cuboid` 和类 `Tetrahedron` 没有将实例添加到父类 `Canvas_3D` 的 bug
+- [X] 修复了当 3D 对象出现在相机位置后面时会显示错误的 bug（目前更改为透视，即不显示）
+- [X] 修复了部分错误的类型提示和错误的参数默认值
+- [X] 移除常量 `BACKGROUND` 并且不再对类 `Canvas` 的默认背景颜色做限定
+
+下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
+* 滚动鼠标中键可以放大和缩小画面；
 * 按“=”和“-”键分别可以放大和缩小几何体的大小；
-* 滚动鼠标中键可以放大和缩小画面。
 
 下面是示例程序的效果图：
 
 ![news.png](news.png)
 
 <details><summary><b>源代码</b></summary>
 
 ```python
-from tkinter import Event
-
 import tkintertools as tkt
 from tkintertools import tools_3d as t3d
 
-root = tkt.Tk('tool_3d', 1280, 720)
-cv3d = t3d.Canvas_3D(root, 1280, 720, 0, 0)
+root = tkt.Tk('tkintertools-2.6.5', 1280, 720)
+cv3d = t3d.Space(root, 1280, 720, 0, 0)
 
-origin = t3d.Point(cv3d, [0, 0, 0])  # 原点
-k = -100, 0, 100
-geos = [t3d.Cuboid(cv3d, a-50, b-50, c-50, 100, 100, 100, color_up='white', color_down='yellow', color_left='red',
-                   color_right='orange', color_front='blue', color_back='green') for a in k for b in k for c in k]
+for a in -100, 0, 100:
+    for b in -100, 0, 100:
+        for c in -100, 0, 100:
+            t3d.Cuboid(cv3d, a-50, b-50, c-50, 100, 100, 100,
+                       color_up='white', color_down='yellow', color_left='red',
+                       color_right='orange', color_front='blue', color_back='green')
 cv3d.space_sort()
 
 
-def translate(event, flag=False, _cache=[]):
-    # type: (Event, bool, list[float]) -> None
-    """ 平移事件 """
-    if flag:
-        _cache[:] = [event.x, event.y]
-        return
-    dx = (event.x - _cache[0])
-    dy = (event.y - _cache[1])
-    _cache[:] = [event.x, event.y]
-    for geo in geos:
-        geo.translate(0, dx, dy)
-        geo.update()
-    origin.translate(0, dx, dy)
-    origin.update()
-    cv3d.space_sort()
-
-
-def rotate(event, flag=False, _cache=[]):
-    # type: (Event, bool, list[float]) -> None
-    """ 旋转事件 """
-    if flag:
-        _cache[:] = [event.x, event.y]
-        return
-    dy = (event.x - _cache[0]) / 100
-    dx = (_cache[1] - event.y) / 100
-    _cache[:] = [event.x, event.y]
-    for item in geos:
-        item.rotate(0, dx, dy, center=origin.coords)
-        item.update()
-    cv3d.space_sort()
-
-
-def scale(event):  # type: (Event) -> None
+def scale(event):
     """ 缩放事件 """
     k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym == 'minus' else 1
-    for geo in geos:
+    for geo in cv3d.geos():
         geo.scale(k, k, k)
         geo.update()
     cv3d.space_sort()
 
 
-def scale_center(event):  # type: (Event) -> None
-    """ 中心缩放事件 """
-    k = 1.05 if event.delta > 0 else 0.95
-    for geo in geos:
-        geo.scale(k, k, k, center=origin.coords)
-        geo.update()
-    cv3d.space_sort()
-
-
-root.bind('<Button-1>', lambda event: rotate(event, True))
-root.bind('<B1-Motion>', rotate)
-root.bind('<Button-3>', lambda event: translate(event, True))
-root.bind('<B3-Motion>', translate)
 root.bind('<Any-Key>', scale)
-root.bind('<MouseWheel>', scale_center)
 root.mainloop()
 ```
 
 </details>
 
 更多更新信息请见：[CHANGELOG.md](CHANGELOG.md)
 
+---
+**特别说明**
+
+    后面的内容即将移植到 Wiki 中！
+
 Description/模块说明
 ----------------------
 
 tkintertools 是一款基于 tkinter 模块的二次开发的界面编程模块，它完全没有使用任何第三方模块和库的，同时，它也没有任何依赖包，它的功能完全由内置模块和函数实现，而且，它还是跨平台的！它和 tkinter 最大的不同在于，它的控件并非真实的控件，而是在 tkinter 模块中 Canvas 对象中绘制而成的，这就赋予了 tkintertools 控件一些在 tkinter 中没有的特性，列举如下：
 
 * 控件背景可以是透明的（实际上是没有背景颜色）
 * 控件的样式可以是自定义的（比如按钮有圆角）
```

#### html2text {}

```diff
@@ -1,82 +1,87 @@
-Metadata-Version: 2.1 Name: tkintertools Version: 2.6.4 Summary: An auxiliary
-module of the tkinder module Home-page: https://github.com/Xiaokang2022/
+Metadata-Version: 2.1 Name: tkintertools Version: 2.6.5 Summary: An auxiliary
+module of the tkinter module Home-page: https://github.com/Xiaokang2022/
 tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com License:
 MulanPSL-2.0 Keywords: tkinter,tkintertools,GUI Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Mulan Permissive
 Software License v2 (MulanPSL-2.0) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.txt
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
-          [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
-                            [Email] [Author] [Blog]
-Installation/æ¨¡åå®è£ -------------------- ### Stable version/ç¨³å®çæ¬
-* Version/çæ¬ : 2.6.4 * Release Date/åå¸æ¥æ : 2023/06/12
-è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
-ï¼å¯è½ï¼æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã å³äºç¨³å®çæ Issue
-çè¯ï¼æä¼å»æ¥çå¹¶å°è¯è§£å³ Issueã ``` pip install
-tkintertools==2.6.4 ``` ### Development version/å¼åçæ¬ * Version/çæ¬ :
-2.6.4 * Release Date/åå¸æ¥æ : 2023/06/11
+             [latest_version] [License] [ChangeLog] [ToDo] [Wiki]
+                      [Downloads] [Author] [Blog] [Email]
+Install/æ¨¡åå®è£ --------------- ### Stable version/ç¨³å®çæ¬ * Version/
+çæ¬ : `2.6.5` * Release Date/åå¸æ¥æ : 2023/06/17 (UTC+08)
+è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bugï¼å¯è½ï¼æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã
+ç¨³å®ç bug
+ä¸ä¸å®å°ï¼ä½å®è³å°æ¯æå¨å¤ä¸ªæä½ç³»ç»ä¸­æµè¯è¿çï¼æ¯è·¨å¹³å°çï¼å¼å®¹çã
+``` pip install tkintertools==2.6.5 ``` ### Development version/å¼åçæ¬ *
+Version/çæ¬ : `2.6.5` * Release Date/åå¸æ¥æ : 2023/06/13 (UTC+08)
 è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼å¯è½ææ°åè½ï¼bug
 ä¹å¯è½ä¼æ¯è¾å¤ï¼ä½ä¹å¯è½ä¼æ¯åæ¥ççæ¬æ´å ç¨³å®ã
-å¤§å®¶å¯ä»¥å¨ Issue
-ä¸­æåºä¸äºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
-``` pip install tkintertools-dev==2.6.4 ``` **ç¹å«æ³¨æ** *
-å¼åçä»ä½ç¤ºä¾ï¼åå½æ°æç±»çAPIå¹¶éæç»ç¡®å®ç»æï¼ç´æ¥ä½¿ç¨å¼åçå¯è½å¯¼è´åç»­æ æ³ä¸æ­£å¼çå¼å®¹ï¼
-*
-è¥è¦ä½¿ç¨å¼åçï¼è¯·åå¸è½½æ­£å¼çååè¿è¡pipå®è£ï¼åæ¬¡ä½¿ç¨æ­£å¼çæ¶ä¹æ¯ä¸æ ·ï¼åå¸è½½å¼åçåå®è£æ­£å¼çï¼
+å¼åçæ²¡æç»è¿å¤æä½ç³»ç»çæµè¯ï¼ä»è½ä¿è¯å¨ Windows
+ç³»ç»ä¸è¿è¡ææåè½ï¼å¨å¶ä»çæä½ç³»ç»ä¸ï¼å¯è½æé¨ååè½æ æ³æ­£å¸¸è¿è¡ã
+å¤§å®¶å¯ä»¥å¨ Issues
+ä¸­æåºä¸äºå»ºè®®ï¼æå¯è½ä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
+``` pip install tkintertools-dev==2.6.5 ``` **Attention/ç¹å«æ³¨æ** *
+å¼åçä»ä½ç¤ºä¾ï¼åå½æ°æç±»ç API
+å¹¶éæç»ç¡®å®ç»æï¼ç´æ¥ä½¿ç¨å¼åçå¯è½å¯¼è´åç»­æ æ³ä¸ç¨³å®çå¼å®¹ï¼
+* è¥è¦ä½¿ç¨å¼åçï¼è¯·åå¸è½½ç¨³å®çååè¿è¡ pip
+å®è£ï¼åæ¬¡ä½¿ç¨ç¨³å®çæ¶ä¹æ¯ä¸æ ·ï¼åå¸è½½å¼åçåå®è£ç¨³å®çï¼
 ### Environmental requirements/ç¯å¢éæ±
-æ²¡æä»»ä½é¢å¤çä¾èµåï¼é¤äºtkinterï¼ï¼ä½åªæ¯æä»¥ä¸ Python
+æ²¡æä»»ä½é¢å¤çä¾èµåï¼é¤äº tkinterï¼ï¼ä½åªæ¯æä»¥ä¸ Python
 çæ¬: ![Python3.8](https://img.shields.io/badge/Python-3.8.*-
 blue?logo=python) ![Python3.9](https://img.shields.io/badge/Python-3.9.*-
 blue?logo=python) ![Python3.10](https://img.shields.io/badge/Python-3.10.*-
 blue?logo=python) ![Python3.11](https://img.shields.io/badge/Python-3.11.*-
 blue?logo=python) ![Python3.12](https://img.shields.io/badge/Python-3.12.*-
 blue?logo=python)
 å¯è½å¨æäºæä½ç³»ç»ä¸ä¹å¯è¿è¡ï¼ä½ç®åä»¥ä¸æä½ç³»ç»å·²ç»æµè¯éè¿:
 ![Windows10](https://img.shields.io/badge/Windows-10-green?logo=windows) !
 [Windows11](https://img.shields.io/badge/Windows-11-green?logo=windows11) !
 [Ubuntu22.04](https://img.shields.io/badge/Ubuntu-22.04-green?logo=ubuntu)
-News/ææ°åè½ ------------ ææ°çç tkintertools **å¼åç**(2.6.4-
-dev)æ°å¢äºå¯¹3då ä½ä½ç©ºé´ä½ç½®æåºçæ¯æï¼ä½¿å¾å ä½ä½ä¸ååªæç²ç¥ççº¿æ¡ï¼èæ¥æä¸°å¯çé¢è²ã
-å¨ Windows ç³»ç»ä¸è¿è¡ä¸é¢çç¤ºä¾ç¨åºæ¶ï¼å¶æ¥æä»¥ä¸åè½ï¼
+News/ææ°åè½ ------------ **ææ°çæ¬: tkintertools-2.6.5 ç¨³å®ç**
+**ãéç£ç¸è£æ´æ°ï¼æ°å¢äº Wiki
+ä¾å¤§å®¶æ¥çï¼æ¹ä¾¿å¤§å®¶è¿éææ¡ tkintertools
+çä½¿ç¨æ¹æ³åå°æå·§ï¼[ç¹æ­¤ä¼ é](https://github.com/Xiaokang2022/
+tkintertools/wiki)ã** ãç¹å«è¯´æã è¿ææ¬äººå°ææ¶åæ­¢å¯¹
+tkintertools æ¨¡åæ¬èº«çæ´æ°ï¼æ¬äººåå»å®å Wiki åç»§ç»­æ´æ°
+tkintertoolsï¼ æ­¤å¤ï¼README.md
+ä¸­å³äºæ¨¡ååå®¹è¯¦ç»ä»ç»çé¨åå°éæ­¥è½¬ç§»å° Wiki ä¸­ï¼
+ä¸é¢æ¯æ¬æ¬¡çæ¬æ´æ°åå®¹æ¡ç®ï¼ - [X] å­æ¨¡å `tools_3d` æ°å¢ç±»
+`Space` å¯ä»¥ç´æ¥æä¾å¯¹ 3D
+å¯¹è±¡è¿è¡å¹³ç§»ãæè½¬åç¼©æ¾ç­æä½çåè½ - [X] ä¿®å¤äºç±»
+`Cuboid` åç±» `Tetrahedron` æ²¡æå°å®ä¾æ·»å å°ç¶ç±» `Canvas_3D` ç
+bug - [X] ä¿®å¤äºå½ 3D
+å¯¹è±¡åºç°å¨ç¸æºä½ç½®åé¢æ¶ä¼æ¾ç¤ºéè¯¯ç
+bugï¼ç®åæ´æ¹ä¸ºéè§ï¼å³ä¸æ¾ç¤ºï¼ - [X]
+ä¿®å¤äºé¨åéè¯¯çç±»åæç¤ºåéè¯¯çåæ°é»è®¤å¼ - [X]
+ç§»é¤å¸¸é `BACKGROUND` å¹¶ä¸ä¸åå¯¹ç±» `Canvas`
+çé»è®¤èæ¯é¢è²åéå®
+ä¸é¢æ¯ä¸ä¸ªä¸»è¦æ°åè½çç¤ºä¾ç¨åºï¼è¿è¡ä¸é¢çç¤ºä¾ç¨åºæ¶ï¼å¶æ¥æä»¥ä¸åè½ï¼
 * æä½é¼ æ å·¦é®æå¨å¯ä»¥æè½¬è¿å¤ä¸ªå ä½ä½ï¼ *
 æä½é¼ æ å³é®æå¨å¯ä»¥ç§»å¨è¿äºå ä½ä½å¨ç©ºé´ä¸­çä½ç½®ï¼ *
-æâ=âåâ-âé®åå«å¯ä»¥æ¾å¤§åç¼©å°å ä½ä½çå¤§å°ï¼ *
-æ»å¨é¼ æ ä¸­é®å¯ä»¥æ¾å¤§åç¼©å°ç»é¢ã
+æ»å¨é¼ æ ä¸­é®å¯ä»¥æ¾å¤§åç¼©å°ç»é¢ï¼ * æâ=âåâ-
+âé®åå«å¯ä»¥æ¾å¤§åç¼©å°å ä½ä½çå¤§å°ï¼
 ä¸é¢æ¯ç¤ºä¾ç¨åºçææå¾ï¼ ![news.png](news.png) æºä»£ç  ```python
-from tkinter import Event import tkintertools as tkt from tkintertools import
-tools_3d as t3d root = tkt.Tk('tool_3d', 1280, 720) cv3d = t3d.Canvas_3D(root,
-1280, 720, 0, 0) origin = t3d.Point(cv3d, [0, 0, 0]) # åç¹ k = -100, 0, 100
-geos = [t3d.Cuboid(cv3d, a-50, b-50, c-50, 100, 100, 100, color_up='white',
-color_down='yellow', color_left='red', color_right='orange',
-color_front='blue', color_back='green') for a in k for b in k for c in k]
-cv3d.space_sort() def translate(event, flag=False, _cache=[]): # type: (Event,
-bool, list[float]) -> None """ å¹³ç§»äºä»¶ """ if flag: _cache[:] = [event.x,
-event.y] return dx = (event.x - _cache[0]) dy = (event.y - _cache[1]) _cache[:
-] = [event.x, event.y] for geo in geos: geo.translate(0, dx, dy) geo.update()
-origin.translate(0, dx, dy) origin.update() cv3d.space_sort() def rotate(event,
-flag=False, _cache=[]): # type: (Event, bool, list[float]) -> None """
-æè½¬äºä»¶ """ if flag: _cache[:] = [event.x, event.y] return dy = (event.x -
-_cache[0]) / 100 dx = (_cache[1] - event.y) / 100 _cache[:] = [event.x,
-event.y] for item in geos: item.rotate(0, dx, dy, center=origin.coords)
-item.update() cv3d.space_sort() def scale(event): # type: (Event) -> None """
-ç¼©æ¾äºä»¶ """ k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym
-== 'minus' else 1 for geo in geos: geo.scale(k, k, k) geo.update()
-cv3d.space_sort() def scale_center(event): # type: (Event) -> None """
-ä¸­å¿ç¼©æ¾äºä»¶ """ k = 1.05 if event.delta > 0 else 0.95 for geo in geos:
-geo.scale(k, k, k, center=origin.coords) geo.update() cv3d.space_sort()
-root.bind('', lambda event: rotate(event, True)) root.bind('', rotate)
-root.bind('', lambda event: translate(event, True)) root.bind('', translate)
-root.bind('', scale) root.bind('', scale_center) root.mainloop() ```
-æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼[CHANGELOG.md](CHANGELOG.md) Description/
-æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº tkinter
+import tkintertools as tkt from tkintertools import tools_3d as t3d root =
+tkt.Tk('tkintertools-2.6.5', 1280, 720) cv3d = t3d.Space(root, 1280, 720, 0, 0)
+for a in -100, 0, 100: for b in -100, 0, 100: for c in -100, 0, 100: t3d.Cuboid
+(cv3d, a-50, b-50, c-50, 100, 100, 100, color_up='white', color_down='yellow',
+color_left='red', color_right='orange', color_front='blue', color_back='green')
+cv3d.space_sort() def scale(event): """ ç¼©æ¾äºä»¶ """ k = 1.05 if
+event.keysym == 'equal' else 0.95 if event.keysym == 'minus' else 1 for geo in
+cv3d.geos(): geo.scale(k, k, k) geo.update() cv3d.space_sort() root.bind('',
+scale) root.mainloop() ```  æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼[CHANGELOG.md]
+(CHANGELOG.md) --- **ç¹å«è¯´æ** åé¢çåå®¹å³å°ç§»æ¤å° Wiki ä¸­ï¼
+Description/æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº
+tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
 tkinter æ¨¡åä¸­ Canvas å¯¹è±¡ä¸­ç»å¶èæçï¼è¿å°±èµäºäº
 tkintertools æ§ä»¶ä¸äºå¨ tkinter ä¸­æ²¡æçç¹æ§ï¼åä¸¾å¦ä¸ï¼ *
 æ§ä»¶èæ¯å¯ä»¥æ¯éæçï¼å®éä¸æ¯æ²¡æèæ¯é¢è²ï¼ *
 æ§ä»¶çæ ·å¼å¯ä»¥æ¯èªå®ä¹çï¼æ¯å¦æé®æåè§ï¼ *
 æ§ä»¶çåå»ºéåº¦è¿å¤§äº tkinter çæ§ä»¶ï¼é¤äº Canvas æ§ä»¶ï¼
```

### Comparing `tkintertools-2.6.4/README.md` & `tkintertools-2.6.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,187 +1,164 @@
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
-    <p><img height="120px" alt="logo.png" src="tkintertools.png" /></p>
+    <p><img height="128px" alt="logo.png" src="tkt.png" /></p>
     <p>
     The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module
     <br />
     <code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块
     </p>
     <p>
-        <a href="tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.4-blue" alt="latest version" />
+        <a href="https://github.com/Xiaokang2022/tkintertools">
+            <img src="https://img.shields.io/badge/Version-2.6.5-blue" alt="latest version" />
         </a>
-        <a href="LICENSE">
+        <a href="LICENSE.txt">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
         <a href="CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/06/12-orange" alt="ChangeLog" />
+            <img src="https://img.shields.io/badge/ChangeLog-2023/06/17-orange" alt="ChangeLog" />
         </a>
         <a href="TODO.md">
-            <img src="https://img.shields.io/badge/ToDo-15-yellow?logo=cachet" alt="ToDos" />
+            <img src="https://img.shields.io/badge/ToDo-14-yellow?logo=cachet" alt="ToDo" />
         </a>
-        <a href="https://pypistats.org/packages/tkintertools">
-            <img src="https://img.shields.io/badge/Download-4k-purple?logo=pypi" alt="Downloads" />
+        <a href="https://github.com/Xiaokang2022/tkintertools/wiki">
+            <img src="https://img.shields.io/badge/Wiki-15-purple" alt="Wiki" />
         </a>
         <br />
-        <a href="mailto:2951256653@qq.com">
-            <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
+        <a href="https://pypistats.org/packages/tkintertools">
+            <img src="https://img.shields.io/badge/Download-6k-white?logo=pypi" alt="Downloads" />
         </a>
         <a href="https://github.com/Xiaokang2022">
-            <img src="https://img.shields.io/badge/Author-小康2022-white" alt="Author" />
+            <img src="https://img.shields.io/badge/Author-小康2022-springgreen" alt="Author" />
         </a>
         <a href="https://xiaokang2022.blog.csdn.net">
             <img src="https://img.shields.io/badge/Blog-小康2022@CSDN-red" alt="Blog" />
         </a>
+        <a href="mailto:2951256653@qq.com">
+            <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
+        </a>
     </p>
 </div>
 
-Installation/模块安装
---------------------
+Install/模块安装
+---------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.4
-* Release Date/发布日期 : 2023/06/12
+* Version/版本 : `2.6.5`
+* Release Date/发布日期 : 2023/06/17 (UTC+08)
 
-这个是目前的最新稳定版，比较稳定，bug （可能）没有那么多，推荐使用这个。  
-关于稳定版有 Issue 的话，我会去查看并尝试解决 Issue。
+这个是目前的最新稳定版，比较稳定，bug（可能）没有那么多，推荐使用这个。  
+稳定版 bug 不一定少，但它至少是我在多个操作系统中测试过的，是跨平台的，兼容的。
 
 ```
-pip install tkintertools==2.6.4
+pip install tkintertools==2.6.5
 ```
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.4
-* Release Date/发布日期 : 2023/06/11
+* Version/版本 : `2.6.5`
+* Release Date/发布日期 : 2023/06/13 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 也可能会比较多，但也可能会比原来的版本更加稳定。  
-大家可以在 Issue 中提出一些建议，我会适当采纳一些并在开发版本中更改或实现。
+开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。  
+大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 ```
-pip install tkintertools-dev==2.6.4
+pip install tkintertools-dev==2.6.5
 ```
 
-**特别注意**
-* 开发版仅作示例，各函数或类的API并非最终确定结果，直接使用开发版可能导致后续无法与正式版兼容！
-* 若要使用开发版，请先卸载正式版后再进行pip安装，再次使用正式版时也是一样，先卸载开发版再安装正式版！
+**Attention/特别注意**
+* 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！
+* 若要使用开发版，请先卸载稳定版后再进行 pip 安装，再次使用稳定版时也是一样，先卸载开发版再安装稳定版！
 
 ### Environmental requirements/环境需求
 
-没有任何额外的依赖包（除了tkinter），但只支持以下 Python 版本:
+没有任何额外的依赖包（除了 tkinter），但只支持以下 Python 版本:
 
 ![Python3.8](https://img.shields.io/badge/Python-3.8.*-blue?logo=python)
 ![Python3.9](https://img.shields.io/badge/Python-3.9.*-blue?logo=python)
 ![Python3.10](https://img.shields.io/badge/Python-3.10.*-blue?logo=python)
 ![Python3.11](https://img.shields.io/badge/Python-3.11.*-blue?logo=python)
 ![Python3.12](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 可能在某些操作系统上也可运行，但目前以下操作系统已经测试通过:
 
 ![Windows10](https://img.shields.io/badge/Windows-10-green?logo=windows)
 ![Windows11](https://img.shields.io/badge/Windows-11-green?logo=windows11)
 ![Ubuntu22.04](https://img.shields.io/badge/Ubuntu-22.04-green?logo=ubuntu)
 
-<a name="news">News/最新功能</a>
+News/最新功能
 ------------
 
-最新版的 tkintertools **开发版**(2.6.4-dev)新增了对3d几何体空间位置排序的支持，使得几何体不再只有粗略的线条，而拥有丰富的颜色。
+**最新版本: tkintertools-2.6.5 稳定版**
 
-在 Windows 系统下运行下面的示例程序时，其拥有以下功能：
+**【重磅炸裂更新：新增了 Wiki 供大家查看，方便大家迅速掌握 tkintertools 的使用方法和小技巧！[点此传送](https://github.com/Xiaokang2022/tkintertools/wiki)】**
+
+    【特别说明】
+    近期本人将暂时停止对 tkintertools 模块本身的更新，本人先去完善 Wiki 再继续更新 tkintertools！
+    此外，README.md 中关于模块内容详细介绍的部分将逐步转移到 Wiki 中！
+
+下面是本次版本更新内容条目：
+
+- [X] 子模块 `tools_3d` 新增类 `Space` 可以直接提供对 3D 对象进行平移、旋转和缩放等操作的功能
+- [X] 修复了类 `Cuboid` 和类 `Tetrahedron` 没有将实例添加到父类 `Canvas_3D` 的 bug
+- [X] 修复了当 3D 对象出现在相机位置后面时会显示错误的 bug（目前更改为透视，即不显示）
+- [X] 修复了部分错误的类型提示和错误的参数默认值
+- [X] 移除常量 `BACKGROUND` 并且不再对类 `Canvas` 的默认背景颜色做限定
+
+下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
+* 滚动鼠标中键可以放大和缩小画面；
 * 按“=”和“-”键分别可以放大和缩小几何体的大小；
-* 滚动鼠标中键可以放大和缩小画面。
 
 下面是示例程序的效果图：
 
 ![news.png](news.png)
 
 <details><summary><b>源代码</b></summary>
 
 ```python
-from tkinter import Event
-
 import tkintertools as tkt
 from tkintertools import tools_3d as t3d
 
-root = tkt.Tk('tool_3d', 1280, 720)
-cv3d = t3d.Canvas_3D(root, 1280, 720, 0, 0)
+root = tkt.Tk('tkintertools-2.6.5', 1280, 720)
+cv3d = t3d.Space(root, 1280, 720, 0, 0)
 
-origin = t3d.Point(cv3d, [0, 0, 0])  # 原点
-k = -100, 0, 100
-geos = [t3d.Cuboid(cv3d, a-50, b-50, c-50, 100, 100, 100, color_up='white', color_down='yellow', color_left='red',
-                   color_right='orange', color_front='blue', color_back='green') for a in k for b in k for c in k]
+for a in -100, 0, 100:
+    for b in -100, 0, 100:
+        for c in -100, 0, 100:
+            t3d.Cuboid(cv3d, a-50, b-50, c-50, 100, 100, 100,
+                       color_up='white', color_down='yellow', color_left='red',
+                       color_right='orange', color_front='blue', color_back='green')
 cv3d.space_sort()
 
 
-def translate(event, flag=False, _cache=[]):
-    # type: (Event, bool, list[float]) -> None
-    """ 平移事件 """
-    if flag:
-        _cache[:] = [event.x, event.y]
-        return
-    dx = (event.x - _cache[0])
-    dy = (event.y - _cache[1])
-    _cache[:] = [event.x, event.y]
-    for geo in geos:
-        geo.translate(0, dx, dy)
-        geo.update()
-    origin.translate(0, dx, dy)
-    origin.update()
-    cv3d.space_sort()
-
-
-def rotate(event, flag=False, _cache=[]):
-    # type: (Event, bool, list[float]) -> None
-    """ 旋转事件 """
-    if flag:
-        _cache[:] = [event.x, event.y]
-        return
-    dy = (event.x - _cache[0]) / 100
-    dx = (_cache[1] - event.y) / 100
-    _cache[:] = [event.x, event.y]
-    for item in geos:
-        item.rotate(0, dx, dy, center=origin.coords)
-        item.update()
-    cv3d.space_sort()
-
-
-def scale(event):  # type: (Event) -> None
+def scale(event):
     """ 缩放事件 """
     k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym == 'minus' else 1
-    for geo in geos:
+    for geo in cv3d.geos():
         geo.scale(k, k, k)
         geo.update()
     cv3d.space_sort()
 
 
-def scale_center(event):  # type: (Event) -> None
-    """ 中心缩放事件 """
-    k = 1.05 if event.delta > 0 else 0.95
-    for geo in geos:
-        geo.scale(k, k, k, center=origin.coords)
-        geo.update()
-    cv3d.space_sort()
-
-
-root.bind('<Button-1>', lambda event: rotate(event, True))
-root.bind('<B1-Motion>', rotate)
-root.bind('<Button-3>', lambda event: translate(event, True))
-root.bind('<B3-Motion>', translate)
 root.bind('<Any-Key>', scale)
-root.bind('<MouseWheel>', scale_center)
 root.mainloop()
 ```
 
 </details>
 
 更多更新信息请见：[CHANGELOG.md](CHANGELOG.md)
 
+---
+**特别说明**
+
+    后面的内容即将移植到 Wiki 中！
+
 Description/模块说明
 ----------------------
 
 tkintertools 是一款基于 tkinter 模块的二次开发的界面编程模块，它完全没有使用任何第三方模块和库的，同时，它也没有任何依赖包，它的功能完全由内置模块和函数实现，而且，它还是跨平台的！它和 tkinter 最大的不同在于，它的控件并非真实的控件，而是在 tkinter 模块中 Canvas 对象中绘制而成的，这就赋予了 tkintertools 控件一些在 tkinter 中没有的特性，列举如下：
 
 * 控件背景可以是透明的（实际上是没有背景颜色）
 * 控件的样式可以是自定义的（比如按钮有圆角）
```

#### html2text {}

```diff
@@ -1,74 +1,79 @@
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
-          [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
-                            [Email] [Author] [Blog]
-Installation/æ¨¡åå®è£ -------------------- ### Stable version/ç¨³å®çæ¬
-* Version/çæ¬ : 2.6.4 * Release Date/åå¸æ¥æ : 2023/06/12
-è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
-ï¼å¯è½ï¼æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã å³äºç¨³å®çæ Issue
-çè¯ï¼æä¼å»æ¥çå¹¶å°è¯è§£å³ Issueã ``` pip install
-tkintertools==2.6.4 ``` ### Development version/å¼åçæ¬ * Version/çæ¬ :
-2.6.4 * Release Date/åå¸æ¥æ : 2023/06/11
+             [latest_version] [License] [ChangeLog] [ToDo] [Wiki]
+                      [Downloads] [Author] [Blog] [Email]
+Install/æ¨¡åå®è£ --------------- ### Stable version/ç¨³å®çæ¬ * Version/
+çæ¬ : `2.6.5` * Release Date/åå¸æ¥æ : 2023/06/17 (UTC+08)
+è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bugï¼å¯è½ï¼æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã
+ç¨³å®ç bug
+ä¸ä¸å®å°ï¼ä½å®è³å°æ¯æå¨å¤ä¸ªæä½ç³»ç»ä¸­æµè¯è¿çï¼æ¯è·¨å¹³å°çï¼å¼å®¹çã
+``` pip install tkintertools==2.6.5 ``` ### Development version/å¼åçæ¬ *
+Version/çæ¬ : `2.6.5` * Release Date/åå¸æ¥æ : 2023/06/13 (UTC+08)
 è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼å¯è½ææ°åè½ï¼bug
 ä¹å¯è½ä¼æ¯è¾å¤ï¼ä½ä¹å¯è½ä¼æ¯åæ¥ççæ¬æ´å ç¨³å®ã
-å¤§å®¶å¯ä»¥å¨ Issue
-ä¸­æåºä¸äºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
-``` pip install tkintertools-dev==2.6.4 ``` **ç¹å«æ³¨æ** *
-å¼åçä»ä½ç¤ºä¾ï¼åå½æ°æç±»çAPIå¹¶éæç»ç¡®å®ç»æï¼ç´æ¥ä½¿ç¨å¼åçå¯è½å¯¼è´åç»­æ æ³ä¸æ­£å¼çå¼å®¹ï¼
-*
-è¥è¦ä½¿ç¨å¼åçï¼è¯·åå¸è½½æ­£å¼çååè¿è¡pipå®è£ï¼åæ¬¡ä½¿ç¨æ­£å¼çæ¶ä¹æ¯ä¸æ ·ï¼åå¸è½½å¼åçåå®è£æ­£å¼çï¼
+å¼åçæ²¡æç»è¿å¤æä½ç³»ç»çæµè¯ï¼ä»è½ä¿è¯å¨ Windows
+ç³»ç»ä¸è¿è¡ææåè½ï¼å¨å¶ä»çæä½ç³»ç»ä¸ï¼å¯è½æé¨ååè½æ æ³æ­£å¸¸è¿è¡ã
+å¤§å®¶å¯ä»¥å¨ Issues
+ä¸­æåºä¸äºå»ºè®®ï¼æå¯è½ä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
+``` pip install tkintertools-dev==2.6.5 ``` **Attention/ç¹å«æ³¨æ** *
+å¼åçä»ä½ç¤ºä¾ï¼åå½æ°æç±»ç API
+å¹¶éæç»ç¡®å®ç»æï¼ç´æ¥ä½¿ç¨å¼åçå¯è½å¯¼è´åç»­æ æ³ä¸ç¨³å®çå¼å®¹ï¼
+* è¥è¦ä½¿ç¨å¼åçï¼è¯·åå¸è½½ç¨³å®çååè¿è¡ pip
+å®è£ï¼åæ¬¡ä½¿ç¨ç¨³å®çæ¶ä¹æ¯ä¸æ ·ï¼åå¸è½½å¼åçåå®è£ç¨³å®çï¼
 ### Environmental requirements/ç¯å¢éæ±
-æ²¡æä»»ä½é¢å¤çä¾èµåï¼é¤äºtkinterï¼ï¼ä½åªæ¯æä»¥ä¸ Python
+æ²¡æä»»ä½é¢å¤çä¾èµåï¼é¤äº tkinterï¼ï¼ä½åªæ¯æä»¥ä¸ Python
 çæ¬: ![Python3.8](https://img.shields.io/badge/Python-3.8.*-
 blue?logo=python) ![Python3.9](https://img.shields.io/badge/Python-3.9.*-
 blue?logo=python) ![Python3.10](https://img.shields.io/badge/Python-3.10.*-
 blue?logo=python) ![Python3.11](https://img.shields.io/badge/Python-3.11.*-
 blue?logo=python) ![Python3.12](https://img.shields.io/badge/Python-3.12.*-
 blue?logo=python)
 å¯è½å¨æäºæä½ç³»ç»ä¸ä¹å¯è¿è¡ï¼ä½ç®åä»¥ä¸æä½ç³»ç»å·²ç»æµè¯éè¿:
 ![Windows10](https://img.shields.io/badge/Windows-10-green?logo=windows) !
 [Windows11](https://img.shields.io/badge/Windows-11-green?logo=windows11) !
 [Ubuntu22.04](https://img.shields.io/badge/Ubuntu-22.04-green?logo=ubuntu)
-News/ææ°åè½ ------------ ææ°çç tkintertools **å¼åç**(2.6.4-
-dev)æ°å¢äºå¯¹3då ä½ä½ç©ºé´ä½ç½®æåºçæ¯æï¼ä½¿å¾å ä½ä½ä¸ååªæç²ç¥ççº¿æ¡ï¼èæ¥æä¸°å¯çé¢è²ã
-å¨ Windows ç³»ç»ä¸è¿è¡ä¸é¢çç¤ºä¾ç¨åºæ¶ï¼å¶æ¥æä»¥ä¸åè½ï¼
+News/ææ°åè½ ------------ **ææ°çæ¬: tkintertools-2.6.5 ç¨³å®ç**
+**ãéç£ç¸è£æ´æ°ï¼æ°å¢äº Wiki
+ä¾å¤§å®¶æ¥çï¼æ¹ä¾¿å¤§å®¶è¿éææ¡ tkintertools
+çä½¿ç¨æ¹æ³åå°æå·§ï¼[ç¹æ­¤ä¼ é](https://github.com/Xiaokang2022/
+tkintertools/wiki)ã** ãç¹å«è¯´æã è¿ææ¬äººå°ææ¶åæ­¢å¯¹
+tkintertools æ¨¡åæ¬èº«çæ´æ°ï¼æ¬äººåå»å®å Wiki åç»§ç»­æ´æ°
+tkintertoolsï¼ æ­¤å¤ï¼README.md
+ä¸­å³äºæ¨¡ååå®¹è¯¦ç»ä»ç»çé¨åå°éæ­¥è½¬ç§»å° Wiki ä¸­ï¼
+ä¸é¢æ¯æ¬æ¬¡çæ¬æ´æ°åå®¹æ¡ç®ï¼ - [X] å­æ¨¡å `tools_3d` æ°å¢ç±»
+`Space` å¯ä»¥ç´æ¥æä¾å¯¹ 3D
+å¯¹è±¡è¿è¡å¹³ç§»ãæè½¬åç¼©æ¾ç­æä½çåè½ - [X] ä¿®å¤äºç±»
+`Cuboid` åç±» `Tetrahedron` æ²¡æå°å®ä¾æ·»å å°ç¶ç±» `Canvas_3D` ç
+bug - [X] ä¿®å¤äºå½ 3D
+å¯¹è±¡åºç°å¨ç¸æºä½ç½®åé¢æ¶ä¼æ¾ç¤ºéè¯¯ç
+bugï¼ç®åæ´æ¹ä¸ºéè§ï¼å³ä¸æ¾ç¤ºï¼ - [X]
+ä¿®å¤äºé¨åéè¯¯çç±»åæç¤ºåéè¯¯çåæ°é»è®¤å¼ - [X]
+ç§»é¤å¸¸é `BACKGROUND` å¹¶ä¸ä¸åå¯¹ç±» `Canvas`
+çé»è®¤èæ¯é¢è²åéå®
+ä¸é¢æ¯ä¸ä¸ªä¸»è¦æ°åè½çç¤ºä¾ç¨åºï¼è¿è¡ä¸é¢çç¤ºä¾ç¨åºæ¶ï¼å¶æ¥æä»¥ä¸åè½ï¼
 * æä½é¼ æ å·¦é®æå¨å¯ä»¥æè½¬è¿å¤ä¸ªå ä½ä½ï¼ *
 æä½é¼ æ å³é®æå¨å¯ä»¥ç§»å¨è¿äºå ä½ä½å¨ç©ºé´ä¸­çä½ç½®ï¼ *
-æâ=âåâ-âé®åå«å¯ä»¥æ¾å¤§åç¼©å°å ä½ä½çå¤§å°ï¼ *
-æ»å¨é¼ æ ä¸­é®å¯ä»¥æ¾å¤§åç¼©å°ç»é¢ã
+æ»å¨é¼ æ ä¸­é®å¯ä»¥æ¾å¤§åç¼©å°ç»é¢ï¼ * æâ=âåâ-
+âé®åå«å¯ä»¥æ¾å¤§åç¼©å°å ä½ä½çå¤§å°ï¼
 ä¸é¢æ¯ç¤ºä¾ç¨åºçææå¾ï¼ ![news.png](news.png) æºä»£ç  ```python
-from tkinter import Event import tkintertools as tkt from tkintertools import
-tools_3d as t3d root = tkt.Tk('tool_3d', 1280, 720) cv3d = t3d.Canvas_3D(root,
-1280, 720, 0, 0) origin = t3d.Point(cv3d, [0, 0, 0]) # åç¹ k = -100, 0, 100
-geos = [t3d.Cuboid(cv3d, a-50, b-50, c-50, 100, 100, 100, color_up='white',
-color_down='yellow', color_left='red', color_right='orange',
-color_front='blue', color_back='green') for a in k for b in k for c in k]
-cv3d.space_sort() def translate(event, flag=False, _cache=[]): # type: (Event,
-bool, list[float]) -> None """ å¹³ç§»äºä»¶ """ if flag: _cache[:] = [event.x,
-event.y] return dx = (event.x - _cache[0]) dy = (event.y - _cache[1]) _cache[:
-] = [event.x, event.y] for geo in geos: geo.translate(0, dx, dy) geo.update()
-origin.translate(0, dx, dy) origin.update() cv3d.space_sort() def rotate(event,
-flag=False, _cache=[]): # type: (Event, bool, list[float]) -> None """
-æè½¬äºä»¶ """ if flag: _cache[:] = [event.x, event.y] return dy = (event.x -
-_cache[0]) / 100 dx = (_cache[1] - event.y) / 100 _cache[:] = [event.x,
-event.y] for item in geos: item.rotate(0, dx, dy, center=origin.coords)
-item.update() cv3d.space_sort() def scale(event): # type: (Event) -> None """
-ç¼©æ¾äºä»¶ """ k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym
-== 'minus' else 1 for geo in geos: geo.scale(k, k, k) geo.update()
-cv3d.space_sort() def scale_center(event): # type: (Event) -> None """
-ä¸­å¿ç¼©æ¾äºä»¶ """ k = 1.05 if event.delta > 0 else 0.95 for geo in geos:
-geo.scale(k, k, k, center=origin.coords) geo.update() cv3d.space_sort()
-root.bind('', lambda event: rotate(event, True)) root.bind('', rotate)
-root.bind('', lambda event: translate(event, True)) root.bind('', translate)
-root.bind('', scale) root.bind('', scale_center) root.mainloop() ```
-æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼[CHANGELOG.md](CHANGELOG.md) Description/
-æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº tkinter
+import tkintertools as tkt from tkintertools import tools_3d as t3d root =
+tkt.Tk('tkintertools-2.6.5', 1280, 720) cv3d = t3d.Space(root, 1280, 720, 0, 0)
+for a in -100, 0, 100: for b in -100, 0, 100: for c in -100, 0, 100: t3d.Cuboid
+(cv3d, a-50, b-50, c-50, 100, 100, 100, color_up='white', color_down='yellow',
+color_left='red', color_right='orange', color_front='blue', color_back='green')
+cv3d.space_sort() def scale(event): """ ç¼©æ¾äºä»¶ """ k = 1.05 if
+event.keysym == 'equal' else 0.95 if event.keysym == 'minus' else 1 for geo in
+cv3d.geos(): geo.scale(k, k, k) geo.update() cv3d.space_sort() root.bind('',
+scale) root.mainloop() ```  æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼[CHANGELOG.md]
+(CHANGELOG.md) --- **ç¹å«è¯´æ** åé¢çåå®¹å³å°ç§»æ¤å° Wiki ä¸­ï¼
+Description/æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº
+tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
 tkinter æ¨¡åä¸­ Canvas å¯¹è±¡ä¸­ç»å¶èæçï¼è¿å°±èµäºäº
 tkintertools æ§ä»¶ä¸äºå¨ tkinter ä¸­æ²¡æçç¹æ§ï¼åä¸¾å¦ä¸ï¼ *
 æ§ä»¶èæ¯å¯ä»¥æ¯éæçï¼å®éä¸æ¯æ²¡æèæ¯é¢è²ï¼ *
 æ§ä»¶çæ ·å¼å¯ä»¥æ¯èªå®ä¹çï¼æ¯å¦æé®æåè§ï¼ *
 æ§ä»¶çåå»ºéåº¦è¿å¤§äº tkinter çæ§ä»¶ï¼é¤äº Canvas æ§ä»¶ï¼
```

### Comparing `tkintertools-2.6.4/setup.py` & `tkintertools-2.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """ 上传 pypi """
 
 import setuptools
 
 setuptools.setup(
     name='tkintertools',
-    version="2.6.4",
+    version='2.6.5',
     author='Xiaokang2022',
     license='MulanPSL-2.0',
     author_email='2951256653@qq.com',
-    description='An auxiliary module of the tkinder module',
+    description='An auxiliary module of the tkinter module',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Xiaokang2022/tkintertools',
     packages=setuptools.find_packages(),
     python_requires='>=3.8',
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `tkintertools-2.6.4/tkintertools/__main__.py` & `tkintertools-2.6.5/tkintertools/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,18 +174,14 @@
         self._widget = []  # type: list[BaseWidget]  # 子控件列表（与事件绑定有关）
         self._font = {}  # type: dict[tkinter._CanvasItemId, float]
         self._image = {}  # type: dict[tkinter._CanvasItemId, list]
 
         tkinter.Canvas.__init__(
             self, master, width=width, height=height, highlightthickness=0, **kw)
 
-        if not (kw.get('bg', None) or kw.get('background', None)):
-            # Linux 系统上背景默认值不是 #F1F1F1，影响模块默认值的效果
-            self.configure(bg=BACKGROUND)
-
         master._canvas.append(self)  # 将实例添加到 Tk 的画布列表中
         if x is not None and y is not None:
             self.place(x=x, y=y)
 
         self.bind('<Motion>', self.__touch)  # 绑定鼠标触碰控件
         self.bind('<Any-Key>', self.__input)  # 绑定键盘输入字符（和Ctrl+v的代码顺序不可错）
         self.bind('<Button-1>', self.__click)  # 绑定鼠标左键按下
```

### Comparing `tkintertools-2.6.4/tkintertools/constants.py` & `tkintertools-2.6.5/tkintertools/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,14 @@
 
 COLOR_NONE = '', '', '', ''
 """ Default transparent color tuple """
 
 COLOR_BAR = '#E1E1E1', '#06b025'
 """ Default progress bar color """
 
-BACKGROUND = '#F1F1F1'
-""" Default Canvas background color """
-
 
 BORDERWIDTH = 1
 """ Default widget borderwidth """
 
 CURSOR = '│'
 """ text cursor """
```

### Comparing `tkintertools-2.6.4/tkintertools/tools_3d.py` & `tkintertools-2.6.5/tkintertools/tools_3d.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ 3D support """
 
 import math  # 数学支持
 import statistics  # 数据统计
+from tkinter import Event  # 类型提示
 from typing import Iterable  # 类型提示
 
 from .__main__ import Canvas, Tk, Toplevel  # 继承和类型提示
 from .constants import *
 
 
 def translate(coords, dx=0, dy=0, dz=0):
@@ -113,46 +114,124 @@
 
     def geos(self):  # type: () -> tuple[Geometry]
         """ 返回`Canvas_3d`类的`geos`元组 """
         return tuple(self._geos)
 
     def space_sort(self):  # type: () -> None
         """ 空间位置排序 """
-        items = [item for item in self._items_3d]
-        items.sort(key=lambda item: item.camera_distance())
-        for item in items:
+        self._items_3d.sort(key=lambda item: item.camera_distance())
+        for item in self._items_3d:
             self.lower(item.item)
 
 
-class _Point():
+class Space(Canvas_3D):
+    """ 三维空间 """
+
+    def __init__(
+        self,
+        master,  # type: Tk | Toplevel
+        width,  # type: int
+        height,  # type: int
+        x=None,  # type: int | None
+        y=None,  # type: int | None
+        *,
+        lock=True,  # type: bool
+        expand=True,  # type: bool
+        keep=True,  # type: bool
+        camera_distance=CAMERA_DISTANCE,  # type: float
+        dx=None,  # type: float | None
+        dy=None,  # type: float | None
+        origin_color='',  # type: str
+        **kw
+    ):  # type: (...) -> None
+        Canvas_3D.__init__(self, master, width, height, x, y, lock=lock, expand=expand,
+                           keep=keep, camera_distance=camera_distance, dx=dx, dy=dy, **kw)
+        self._origin = Point(self, [0, 0, 0], size=1,
+                             fill=origin_color, outline=origin_color)
+        self.space_sort()
+        self.bind('<B3-Motion>', self._translate)
+        self.bind('<Button-3>', lambda _: self._translate(_, True))
+        self.bind('<ButtonRelease-3>', lambda _: self._translate(_, False))
+        self.bind('<B1-Motion>', self._rotate)
+        self.bind('<Button-1>', lambda _: self._rotate(_, True))
+        self.bind('<ButtonRelease-1>', lambda _: self._rotate(_, False))
+        if SYSTEM == 'Linux':  # 兼容 Linux 系统
+            self.bind('<Button-4>', lambda _: self._zoom(_, True))
+            self.bind('<Button-5>', lambda _: self._zoom(_, False))
+        else:
+            self.bind('<MouseWheel>', self._zoom)
+
+    def _translate(self, event, flag=None, cache=[]):
+        # type: (Event, bool | None, list[float]) -> None
+        """ 平移视角 """
+        if flag is True:  # 按下
+            cache[:] = [event.x, event.y]
+            return self.configure(cursor='fleur')
+        elif flag is False:  # 松开
+            return self.configure(cursor='arrow')
+        dx, dy = event.x-cache[0], event.y-cache[1]
+        cache[:] = [event.x, event.y]
+        for item in self._geos+[self._origin]:
+            item.translate(0, dx, dy)
+            item.update()
+        self.space_sort()
+
+    def _rotate(self, event, flag=None, cache=[]):
+        # type: (Event, bool | None, list[float]) -> None
+        """ 旋转视角 """
+        if flag is True:
+            cache[:] = [event.x, event.y]
+            return self.configure(cursor='fleur')
+        elif flag is False:
+            return self.configure(cursor='arrow')
+        dx, dy = event.x-cache[0], event.y-cache[1]
+        cache[:] = [event.x, event.y]
+        for item in self._geos+[self._origin]:
+            item.rotate(0, -dy/self.dx*math.pi, dx /
+                        self.dy*math.pi, center=self._origin.coords)
+            item.update()
+        self.space_sort()
+
+    def _zoom(self, event, flag=None):  # type: (Event, bool | None) -> None
+        """ 缩放视角 """
+        if flag is not None:
+            event.delta = flag
+        k = 1.1 if event.delta > 0 else 0.9
+        for item in self.geos():
+            item.scale(k, k, k, center=self._origin.coords)
+            item.update()
+        self.space_sort()
+
+
+class _Point:
     """ 点 """
 
     def __init__(self, coords):  # type: (list[float]) -> None
         self.coords = coords  # 利用列表引用
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
         """ 平移 """
         translate(self.coords, dx, dy, dz)
 
-    def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0], axes=None, delta=0):
-        # type: (float, float, float, ..., Iterable[float], Line | None, float) -> None
+    def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
+        # type: (float, float, float, ..., Iterable[float]) -> None
         """ 旋转 """
-        rotate(self.coords, dx, dy, dz, center=center, axes=axes, delta=delta)
+        rotate(self.coords, dx, dy, dz, center=center)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., Iterable[float] | None) -> None
         """ 缩放 """
         scale(self.coords, kx, ky, kz, center=center)
 
     def project(self, distance):  # type: (float) -> list[float]
         """ 投影 """
-        try:
-            k = distance/(distance - self.coords[0])
-        except ZeroDivisionError:
-            return [distance*10, distance*10]
+        relative_dis = distance - self.coords[0]
+        if relative_dis <= 1e-16:
+            return [float('INF')]*2  # BUG
+        k = distance/relative_dis
         return [self.coords[1]*k, self.coords[2]*k]
 
 
 class _Line:
     """ 线 """
 
     def __init__(
@@ -373,15 +452,15 @@
         `dz`: z轴方向位移距离\n
         """
         coords = [coord for side in self.sides for coord in side.coords]
         for ind, coord in enumerate(coords):
             if coord not in coords[:ind]:
                 translate(coord, dx, dy, dz)
 
-    def rotate(self, dx=1, dy=1, dz=1, *, center=[0, 0, 0]):
+    def rotate(self, dx=0, dy=0, dz=0, *, center=[0, 0, 0]):
         # type: (float, float, float, ..., Iterable[float]) -> None
         """
         旋转\n
         `dx`: 绕x轴方向旋转弧度\n
         `dy`: 绕y轴方向旋转弧度\n
         `dz`: 绕z轴方向旋转弧度\n
         `center`: 旋转中心\n
@@ -456,14 +535,15 @@
         `color_up`: 上表面颜色\n
         `color_down`: 下表面颜色\n
         `color_left`: 左侧面颜色\n
         `color_right`: 右侧面颜色\n
         `color_front`: 正面颜色\n
         `color_back`: 后面颜色\n
         """
+        canvas._geos.append(self)
         self.canvas = canvas
         self.coords = [[x+l, y+w, z+h]
                        for l in (0, length)
                        for w in (0, width)
                        for h in (0, height)]
         self.sides = [
             Side(canvas, self.coords[0], self.coords[1],
@@ -498,14 +578,15 @@
         `canvas`: 父画布\n
         `p1`: 第一个顶点\n
         `p2`: 第二个顶点\n
         `p3`: 第三个顶点\n
         `p4`: 第四个顶点\n
         `colors`: 颜色序列\n
         """
+        canvas._geos.append(self)
         self.canvas = canvas
         self.coords = [list(p1), list(p2), list(p3), list(p4)]
         self.sides = [
             Side(canvas, self.coords[0], self.coords[1],
                  self.coords[2], fill=colors[0]),
             Side(canvas, self.coords[0], self.coords[1],
                  self.coords[3], fill=colors[1]),
```

### Comparing `tkintertools-2.6.4/tkintertools.egg-info/PKG-INFO` & `tkintertools-2.6.5/tkintertools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,203 +1,180 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.4
-Summary: An auxiliary module of the tkinder module
+Version: 2.6.5
+Summary: An auxiliary module of the tkinter module
 Home-page: https://github.com/Xiaokang2022/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 License: MulanPSL-2.0
 Keywords: tkinter,tkintertools,GUI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.txt
 
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
-    <p><img height="120px" alt="logo.png" src="tkintertools.png" /></p>
+    <p><img height="128px" alt="logo.png" src="tkt.png" /></p>
     <p>
     The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module
     <br />
     <code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块
     </p>
     <p>
-        <a href="tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.4-blue" alt="latest version" />
+        <a href="https://github.com/Xiaokang2022/tkintertools">
+            <img src="https://img.shields.io/badge/Version-2.6.5-blue" alt="latest version" />
         </a>
-        <a href="LICENSE">
+        <a href="LICENSE.txt">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
         <a href="CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/06/12-orange" alt="ChangeLog" />
+            <img src="https://img.shields.io/badge/ChangeLog-2023/06/17-orange" alt="ChangeLog" />
         </a>
         <a href="TODO.md">
-            <img src="https://img.shields.io/badge/ToDo-15-yellow?logo=cachet" alt="ToDos" />
+            <img src="https://img.shields.io/badge/ToDo-14-yellow?logo=cachet" alt="ToDo" />
         </a>
-        <a href="https://pypistats.org/packages/tkintertools">
-            <img src="https://img.shields.io/badge/Download-4k-purple?logo=pypi" alt="Downloads" />
+        <a href="https://github.com/Xiaokang2022/tkintertools/wiki">
+            <img src="https://img.shields.io/badge/Wiki-15-purple" alt="Wiki" />
         </a>
         <br />
-        <a href="mailto:2951256653@qq.com">
-            <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
+        <a href="https://pypistats.org/packages/tkintertools">
+            <img src="https://img.shields.io/badge/Download-6k-white?logo=pypi" alt="Downloads" />
         </a>
         <a href="https://github.com/Xiaokang2022">
-            <img src="https://img.shields.io/badge/Author-小康2022-white" alt="Author" />
+            <img src="https://img.shields.io/badge/Author-小康2022-springgreen" alt="Author" />
         </a>
         <a href="https://xiaokang2022.blog.csdn.net">
             <img src="https://img.shields.io/badge/Blog-小康2022@CSDN-red" alt="Blog" />
         </a>
+        <a href="mailto:2951256653@qq.com">
+            <img src="https://img.shields.io/badge/Email-2951256653@qq.com-cyan" alt="Email" />
+        </a>
     </p>
 </div>
 
-Installation/模块安装
---------------------
+Install/模块安装
+---------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.4
-* Release Date/发布日期 : 2023/06/12
+* Version/版本 : `2.6.5`
+* Release Date/发布日期 : 2023/06/17 (UTC+08)
 
-这个是目前的最新稳定版，比较稳定，bug （可能）没有那么多，推荐使用这个。  
-关于稳定版有 Issue 的话，我会去查看并尝试解决 Issue。
+这个是目前的最新稳定版，比较稳定，bug（可能）没有那么多，推荐使用这个。  
+稳定版 bug 不一定少，但它至少是我在多个操作系统中测试过的，是跨平台的，兼容的。
 
 ```
-pip install tkintertools==2.6.4
+pip install tkintertools==2.6.5
 ```
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.4
-* Release Date/发布日期 : 2023/06/11
+* Version/版本 : `2.6.5`
+* Release Date/发布日期 : 2023/06/13 (UTC+08)
 
 这个是我正在开发的版本，可能有新功能，bug 也可能会比较多，但也可能会比原来的版本更加稳定。  
-大家可以在 Issue 中提出一些建议，我会适当采纳一些并在开发版本中更改或实现。
+开发版没有经过多操作系统的测试，仅能保证在 Windows 系统下运行所有功能，在其他的操作系统上，可能有部分功能无法正常运行。  
+大家可以在 Issues 中提出一些建议，我可能会适当采纳一些并在开发版本中更改或实现。
 
 ```
-pip install tkintertools-dev==2.6.4
+pip install tkintertools-dev==2.6.5
 ```
 
-**特别注意**
-* 开发版仅作示例，各函数或类的API并非最终确定结果，直接使用开发版可能导致后续无法与正式版兼容！
-* 若要使用开发版，请先卸载正式版后再进行pip安装，再次使用正式版时也是一样，先卸载开发版再安装正式版！
+**Attention/特别注意**
+* 开发版仅作示例，各函数或类的 API 并非最终确定结果，直接使用开发版可能导致后续无法与稳定版兼容！
+* 若要使用开发版，请先卸载稳定版后再进行 pip 安装，再次使用稳定版时也是一样，先卸载开发版再安装稳定版！
 
 ### Environmental requirements/环境需求
 
-没有任何额外的依赖包（除了tkinter），但只支持以下 Python 版本:
+没有任何额外的依赖包（除了 tkinter），但只支持以下 Python 版本:
 
 ![Python3.8](https://img.shields.io/badge/Python-3.8.*-blue?logo=python)
 ![Python3.9](https://img.shields.io/badge/Python-3.9.*-blue?logo=python)
 ![Python3.10](https://img.shields.io/badge/Python-3.10.*-blue?logo=python)
 ![Python3.11](https://img.shields.io/badge/Python-3.11.*-blue?logo=python)
 ![Python3.12](https://img.shields.io/badge/Python-3.12.*-blue?logo=python)
 
 可能在某些操作系统上也可运行，但目前以下操作系统已经测试通过:
 
 ![Windows10](https://img.shields.io/badge/Windows-10-green?logo=windows)
 ![Windows11](https://img.shields.io/badge/Windows-11-green?logo=windows11)
 ![Ubuntu22.04](https://img.shields.io/badge/Ubuntu-22.04-green?logo=ubuntu)
 
-<a name="news">News/最新功能</a>
+News/最新功能
 ------------
 
-最新版的 tkintertools **开发版**(2.6.4-dev)新增了对3d几何体空间位置排序的支持，使得几何体不再只有粗略的线条，而拥有丰富的颜色。
+**最新版本: tkintertools-2.6.5 稳定版**
 
-在 Windows 系统下运行下面的示例程序时，其拥有以下功能：
+**【重磅炸裂更新：新增了 Wiki 供大家查看，方便大家迅速掌握 tkintertools 的使用方法和小技巧！[点此传送](https://github.com/Xiaokang2022/tkintertools/wiki)】**
+
+    【特别说明】
+    近期本人将暂时停止对 tkintertools 模块本身的更新，本人先去完善 Wiki 再继续更新 tkintertools！
+    此外，README.md 中关于模块内容详细介绍的部分将逐步转移到 Wiki 中！
+
+下面是本次版本更新内容条目：
+
+- [X] 子模块 `tools_3d` 新增类 `Space` 可以直接提供对 3D 对象进行平移、旋转和缩放等操作的功能
+- [X] 修复了类 `Cuboid` 和类 `Tetrahedron` 没有将实例添加到父类 `Canvas_3D` 的 bug
+- [X] 修复了当 3D 对象出现在相机位置后面时会显示错误的 bug（目前更改为透视，即不显示）
+- [X] 修复了部分错误的类型提示和错误的参数默认值
+- [X] 移除常量 `BACKGROUND` 并且不再对类 `Canvas` 的默认背景颜色做限定
+
+下面是一个主要新功能的示例程序，运行下面的示例程序时，其拥有以下功能：
 * 按住鼠标左键拖动可以旋转这多个几何体；
 * 按住鼠标右键拖动可以移动这些几何体在空间中的位置；
+* 滚动鼠标中键可以放大和缩小画面；
 * 按“=”和“-”键分别可以放大和缩小几何体的大小；
-* 滚动鼠标中键可以放大和缩小画面。
 
 下面是示例程序的效果图：
 
 ![news.png](news.png)
 
 <details><summary><b>源代码</b></summary>
 
 ```python
-from tkinter import Event
-
 import tkintertools as tkt
 from tkintertools import tools_3d as t3d
 
-root = tkt.Tk('tool_3d', 1280, 720)
-cv3d = t3d.Canvas_3D(root, 1280, 720, 0, 0)
+root = tkt.Tk('tkintertools-2.6.5', 1280, 720)
+cv3d = t3d.Space(root, 1280, 720, 0, 0)
 
-origin = t3d.Point(cv3d, [0, 0, 0])  # 原点
-k = -100, 0, 100
-geos = [t3d.Cuboid(cv3d, a-50, b-50, c-50, 100, 100, 100, color_up='white', color_down='yellow', color_left='red',
-                   color_right='orange', color_front='blue', color_back='green') for a in k for b in k for c in k]
+for a in -100, 0, 100:
+    for b in -100, 0, 100:
+        for c in -100, 0, 100:
+            t3d.Cuboid(cv3d, a-50, b-50, c-50, 100, 100, 100,
+                       color_up='white', color_down='yellow', color_left='red',
+                       color_right='orange', color_front='blue', color_back='green')
 cv3d.space_sort()
 
 
-def translate(event, flag=False, _cache=[]):
-    # type: (Event, bool, list[float]) -> None
-    """ 平移事件 """
-    if flag:
-        _cache[:] = [event.x, event.y]
-        return
-    dx = (event.x - _cache[0])
-    dy = (event.y - _cache[1])
-    _cache[:] = [event.x, event.y]
-    for geo in geos:
-        geo.translate(0, dx, dy)
-        geo.update()
-    origin.translate(0, dx, dy)
-    origin.update()
-    cv3d.space_sort()
-
-
-def rotate(event, flag=False, _cache=[]):
-    # type: (Event, bool, list[float]) -> None
-    """ 旋转事件 """
-    if flag:
-        _cache[:] = [event.x, event.y]
-        return
-    dy = (event.x - _cache[0]) / 100
-    dx = (_cache[1] - event.y) / 100
-    _cache[:] = [event.x, event.y]
-    for item in geos:
-        item.rotate(0, dx, dy, center=origin.coords)
-        item.update()
-    cv3d.space_sort()
-
-
-def scale(event):  # type: (Event) -> None
+def scale(event):
     """ 缩放事件 """
     k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym == 'minus' else 1
-    for geo in geos:
+    for geo in cv3d.geos():
         geo.scale(k, k, k)
         geo.update()
     cv3d.space_sort()
 
 
-def scale_center(event):  # type: (Event) -> None
-    """ 中心缩放事件 """
-    k = 1.05 if event.delta > 0 else 0.95
-    for geo in geos:
-        geo.scale(k, k, k, center=origin.coords)
-        geo.update()
-    cv3d.space_sort()
-
-
-root.bind('<Button-1>', lambda event: rotate(event, True))
-root.bind('<B1-Motion>', rotate)
-root.bind('<Button-3>', lambda event: translate(event, True))
-root.bind('<B3-Motion>', translate)
 root.bind('<Any-Key>', scale)
-root.bind('<MouseWheel>', scale_center)
 root.mainloop()
 ```
 
 </details>
 
 更多更新信息请见：[CHANGELOG.md](CHANGELOG.md)
 
+---
+**特别说明**
+
+    后面的内容即将移植到 Wiki 中！
+
 Description/模块说明
 ----------------------
 
 tkintertools 是一款基于 tkinter 模块的二次开发的界面编程模块，它完全没有使用任何第三方模块和库的，同时，它也没有任何依赖包，它的功能完全由内置模块和函数实现，而且，它还是跨平台的！它和 tkinter 最大的不同在于，它的控件并非真实的控件，而是在 tkinter 模块中 Canvas 对象中绘制而成的，这就赋予了 tkintertools 控件一些在 tkinter 中没有的特性，列举如下：
 
 * 控件背景可以是透明的（实际上是没有背景颜色）
 * 控件的样式可以是自定义的（比如按钮有圆角）
```

#### html2text {}

```diff
@@ -1,82 +1,87 @@
-Metadata-Version: 2.1 Name: tkintertools Version: 2.6.4 Summary: An auxiliary
-module of the tkinder module Home-page: https://github.com/Xiaokang2022/
+Metadata-Version: 2.1 Name: tkintertools Version: 2.6.5 Summary: An auxiliary
+module of the tkinter module Home-page: https://github.com/Xiaokang2022/
 tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com License:
 MulanPSL-2.0 Keywords: tkinter,tkintertools,GUI Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Mulan Permissive
 Software License v2 (MulanPSL-2.0) Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.txt
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
-          [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
-                            [Email] [Author] [Blog]
-Installation/æ¨¡åå®è£ -------------------- ### Stable version/ç¨³å®çæ¬
-* Version/çæ¬ : 2.6.4 * Release Date/åå¸æ¥æ : 2023/06/12
-è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
-ï¼å¯è½ï¼æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã å³äºç¨³å®çæ Issue
-çè¯ï¼æä¼å»æ¥çå¹¶å°è¯è§£å³ Issueã ``` pip install
-tkintertools==2.6.4 ``` ### Development version/å¼åçæ¬ * Version/çæ¬ :
-2.6.4 * Release Date/åå¸æ¥æ : 2023/06/11
+             [latest_version] [License] [ChangeLog] [ToDo] [Wiki]
+                      [Downloads] [Author] [Blog] [Email]
+Install/æ¨¡åå®è£ --------------- ### Stable version/ç¨³å®çæ¬ * Version/
+çæ¬ : `2.6.5` * Release Date/åå¸æ¥æ : 2023/06/17 (UTC+08)
+è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bugï¼å¯è½ï¼æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã
+ç¨³å®ç bug
+ä¸ä¸å®å°ï¼ä½å®è³å°æ¯æå¨å¤ä¸ªæä½ç³»ç»ä¸­æµè¯è¿çï¼æ¯è·¨å¹³å°çï¼å¼å®¹çã
+``` pip install tkintertools==2.6.5 ``` ### Development version/å¼åçæ¬ *
+Version/çæ¬ : `2.6.5` * Release Date/åå¸æ¥æ : 2023/06/13 (UTC+08)
 è¿ä¸ªæ¯ææ­£å¨å¼åççæ¬ï¼å¯è½ææ°åè½ï¼bug
 ä¹å¯è½ä¼æ¯è¾å¤ï¼ä½ä¹å¯è½ä¼æ¯åæ¥ççæ¬æ´å ç¨³å®ã
-å¤§å®¶å¯ä»¥å¨ Issue
-ä¸­æåºä¸äºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
-``` pip install tkintertools-dev==2.6.4 ``` **ç¹å«æ³¨æ** *
-å¼åçä»ä½ç¤ºä¾ï¼åå½æ°æç±»çAPIå¹¶éæç»ç¡®å®ç»æï¼ç´æ¥ä½¿ç¨å¼åçå¯è½å¯¼è´åç»­æ æ³ä¸æ­£å¼çå¼å®¹ï¼
-*
-è¥è¦ä½¿ç¨å¼åçï¼è¯·åå¸è½½æ­£å¼çååè¿è¡pipå®è£ï¼åæ¬¡ä½¿ç¨æ­£å¼çæ¶ä¹æ¯ä¸æ ·ï¼åå¸è½½å¼åçåå®è£æ­£å¼çï¼
+å¼åçæ²¡æç»è¿å¤æä½ç³»ç»çæµè¯ï¼ä»è½ä¿è¯å¨ Windows
+ç³»ç»ä¸è¿è¡ææåè½ï¼å¨å¶ä»çæä½ç³»ç»ä¸ï¼å¯è½æé¨ååè½æ æ³æ­£å¸¸è¿è¡ã
+å¤§å®¶å¯ä»¥å¨ Issues
+ä¸­æåºä¸äºå»ºè®®ï¼æå¯è½ä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
+``` pip install tkintertools-dev==2.6.5 ``` **Attention/ç¹å«æ³¨æ** *
+å¼åçä»ä½ç¤ºä¾ï¼åå½æ°æç±»ç API
+å¹¶éæç»ç¡®å®ç»æï¼ç´æ¥ä½¿ç¨å¼åçå¯è½å¯¼è´åç»­æ æ³ä¸ç¨³å®çå¼å®¹ï¼
+* è¥è¦ä½¿ç¨å¼åçï¼è¯·åå¸è½½ç¨³å®çååè¿è¡ pip
+å®è£ï¼åæ¬¡ä½¿ç¨ç¨³å®çæ¶ä¹æ¯ä¸æ ·ï¼åå¸è½½å¼åçåå®è£ç¨³å®çï¼
 ### Environmental requirements/ç¯å¢éæ±
-æ²¡æä»»ä½é¢å¤çä¾èµåï¼é¤äºtkinterï¼ï¼ä½åªæ¯æä»¥ä¸ Python
+æ²¡æä»»ä½é¢å¤çä¾èµåï¼é¤äº tkinterï¼ï¼ä½åªæ¯æä»¥ä¸ Python
 çæ¬: ![Python3.8](https://img.shields.io/badge/Python-3.8.*-
 blue?logo=python) ![Python3.9](https://img.shields.io/badge/Python-3.9.*-
 blue?logo=python) ![Python3.10](https://img.shields.io/badge/Python-3.10.*-
 blue?logo=python) ![Python3.11](https://img.shields.io/badge/Python-3.11.*-
 blue?logo=python) ![Python3.12](https://img.shields.io/badge/Python-3.12.*-
 blue?logo=python)
 å¯è½å¨æäºæä½ç³»ç»ä¸ä¹å¯è¿è¡ï¼ä½ç®åä»¥ä¸æä½ç³»ç»å·²ç»æµè¯éè¿:
 ![Windows10](https://img.shields.io/badge/Windows-10-green?logo=windows) !
 [Windows11](https://img.shields.io/badge/Windows-11-green?logo=windows11) !
 [Ubuntu22.04](https://img.shields.io/badge/Ubuntu-22.04-green?logo=ubuntu)
-News/ææ°åè½ ------------ ææ°çç tkintertools **å¼åç**(2.6.4-
-dev)æ°å¢äºå¯¹3då ä½ä½ç©ºé´ä½ç½®æåºçæ¯æï¼ä½¿å¾å ä½ä½ä¸ååªæç²ç¥ççº¿æ¡ï¼èæ¥æä¸°å¯çé¢è²ã
-å¨ Windows ç³»ç»ä¸è¿è¡ä¸é¢çç¤ºä¾ç¨åºæ¶ï¼å¶æ¥æä»¥ä¸åè½ï¼
+News/ææ°åè½ ------------ **ææ°çæ¬: tkintertools-2.6.5 ç¨³å®ç**
+**ãéç£ç¸è£æ´æ°ï¼æ°å¢äº Wiki
+ä¾å¤§å®¶æ¥çï¼æ¹ä¾¿å¤§å®¶è¿éææ¡ tkintertools
+çä½¿ç¨æ¹æ³åå°æå·§ï¼[ç¹æ­¤ä¼ é](https://github.com/Xiaokang2022/
+tkintertools/wiki)ã** ãç¹å«è¯´æã è¿ææ¬äººå°ææ¶åæ­¢å¯¹
+tkintertools æ¨¡åæ¬èº«çæ´æ°ï¼æ¬äººåå»å®å Wiki åç»§ç»­æ´æ°
+tkintertoolsï¼ æ­¤å¤ï¼README.md
+ä¸­å³äºæ¨¡ååå®¹è¯¦ç»ä»ç»çé¨åå°éæ­¥è½¬ç§»å° Wiki ä¸­ï¼
+ä¸é¢æ¯æ¬æ¬¡çæ¬æ´æ°åå®¹æ¡ç®ï¼ - [X] å­æ¨¡å `tools_3d` æ°å¢ç±»
+`Space` å¯ä»¥ç´æ¥æä¾å¯¹ 3D
+å¯¹è±¡è¿è¡å¹³ç§»ãæè½¬åç¼©æ¾ç­æä½çåè½ - [X] ä¿®å¤äºç±»
+`Cuboid` åç±» `Tetrahedron` æ²¡æå°å®ä¾æ·»å å°ç¶ç±» `Canvas_3D` ç
+bug - [X] ä¿®å¤äºå½ 3D
+å¯¹è±¡åºç°å¨ç¸æºä½ç½®åé¢æ¶ä¼æ¾ç¤ºéè¯¯ç
+bugï¼ç®åæ´æ¹ä¸ºéè§ï¼å³ä¸æ¾ç¤ºï¼ - [X]
+ä¿®å¤äºé¨åéè¯¯çç±»åæç¤ºåéè¯¯çåæ°é»è®¤å¼ - [X]
+ç§»é¤å¸¸é `BACKGROUND` å¹¶ä¸ä¸åå¯¹ç±» `Canvas`
+çé»è®¤èæ¯é¢è²åéå®
+ä¸é¢æ¯ä¸ä¸ªä¸»è¦æ°åè½çç¤ºä¾ç¨åºï¼è¿è¡ä¸é¢çç¤ºä¾ç¨åºæ¶ï¼å¶æ¥æä»¥ä¸åè½ï¼
 * æä½é¼ æ å·¦é®æå¨å¯ä»¥æè½¬è¿å¤ä¸ªå ä½ä½ï¼ *
 æä½é¼ æ å³é®æå¨å¯ä»¥ç§»å¨è¿äºå ä½ä½å¨ç©ºé´ä¸­çä½ç½®ï¼ *
-æâ=âåâ-âé®åå«å¯ä»¥æ¾å¤§åç¼©å°å ä½ä½çå¤§å°ï¼ *
-æ»å¨é¼ æ ä¸­é®å¯ä»¥æ¾å¤§åç¼©å°ç»é¢ã
+æ»å¨é¼ æ ä¸­é®å¯ä»¥æ¾å¤§åç¼©å°ç»é¢ï¼ * æâ=âåâ-
+âé®åå«å¯ä»¥æ¾å¤§åç¼©å°å ä½ä½çå¤§å°ï¼
 ä¸é¢æ¯ç¤ºä¾ç¨åºçææå¾ï¼ ![news.png](news.png) æºä»£ç  ```python
-from tkinter import Event import tkintertools as tkt from tkintertools import
-tools_3d as t3d root = tkt.Tk('tool_3d', 1280, 720) cv3d = t3d.Canvas_3D(root,
-1280, 720, 0, 0) origin = t3d.Point(cv3d, [0, 0, 0]) # åç¹ k = -100, 0, 100
-geos = [t3d.Cuboid(cv3d, a-50, b-50, c-50, 100, 100, 100, color_up='white',
-color_down='yellow', color_left='red', color_right='orange',
-color_front='blue', color_back='green') for a in k for b in k for c in k]
-cv3d.space_sort() def translate(event, flag=False, _cache=[]): # type: (Event,
-bool, list[float]) -> None """ å¹³ç§»äºä»¶ """ if flag: _cache[:] = [event.x,
-event.y] return dx = (event.x - _cache[0]) dy = (event.y - _cache[1]) _cache[:
-] = [event.x, event.y] for geo in geos: geo.translate(0, dx, dy) geo.update()
-origin.translate(0, dx, dy) origin.update() cv3d.space_sort() def rotate(event,
-flag=False, _cache=[]): # type: (Event, bool, list[float]) -> None """
-æè½¬äºä»¶ """ if flag: _cache[:] = [event.x, event.y] return dy = (event.x -
-_cache[0]) / 100 dx = (_cache[1] - event.y) / 100 _cache[:] = [event.x,
-event.y] for item in geos: item.rotate(0, dx, dy, center=origin.coords)
-item.update() cv3d.space_sort() def scale(event): # type: (Event) -> None """
-ç¼©æ¾äºä»¶ """ k = 1.05 if event.keysym == 'equal' else 0.95 if event.keysym
-== 'minus' else 1 for geo in geos: geo.scale(k, k, k) geo.update()
-cv3d.space_sort() def scale_center(event): # type: (Event) -> None """
-ä¸­å¿ç¼©æ¾äºä»¶ """ k = 1.05 if event.delta > 0 else 0.95 for geo in geos:
-geo.scale(k, k, k, center=origin.coords) geo.update() cv3d.space_sort()
-root.bind('', lambda event: rotate(event, True)) root.bind('', rotate)
-root.bind('', lambda event: translate(event, True)) root.bind('', translate)
-root.bind('', scale) root.bind('', scale_center) root.mainloop() ```
-æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼[CHANGELOG.md](CHANGELOG.md) Description/
-æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº tkinter
+import tkintertools as tkt from tkintertools import tools_3d as t3d root =
+tkt.Tk('tkintertools-2.6.5', 1280, 720) cv3d = t3d.Space(root, 1280, 720, 0, 0)
+for a in -100, 0, 100: for b in -100, 0, 100: for c in -100, 0, 100: t3d.Cuboid
+(cv3d, a-50, b-50, c-50, 100, 100, 100, color_up='white', color_down='yellow',
+color_left='red', color_right='orange', color_front='blue', color_back='green')
+cv3d.space_sort() def scale(event): """ ç¼©æ¾äºä»¶ """ k = 1.05 if
+event.keysym == 'equal' else 0.95 if event.keysym == 'minus' else 1 for geo in
+cv3d.geos(): geo.scale(k, k, k) geo.update() cv3d.space_sort() root.bind('',
+scale) root.mainloop() ```  æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼[CHANGELOG.md]
+(CHANGELOG.md) --- **ç¹å«è¯´æ** åé¢çåå®¹å³å°ç§»æ¤å° Wiki ä¸­ï¼
+Description/æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº
+tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
 tkinter æ¨¡åä¸­ Canvas å¯¹è±¡ä¸­ç»å¶èæçï¼è¿å°±èµäºäº
 tkintertools æ§ä»¶ä¸äºå¨ tkinter ä¸­æ²¡æçç¹æ§ï¼åä¸¾å¦ä¸ï¼ *
 æ§ä»¶èæ¯å¯ä»¥æ¯éæçï¼å®éä¸æ¯æ²¡æèæ¯é¢è²ï¼ *
 æ§ä»¶çæ ·å¼å¯ä»¥æ¯èªå®ä¹çï¼æ¯å¦æé®æåè§ï¼ *
 æ§ä»¶çåå»ºéåº¦è¿å¤§äº tkinter çæ§ä»¶ï¼é¤äº Canvas æ§ä»¶ï¼
```

