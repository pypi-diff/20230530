# Comparing `tmp/tkintertools-2.6.1.2.tar.gz` & `tmp/tkintertools-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-2.6.1.2.tar", last modified: Mon May 22 14:07:59 2023, max compression
+gzip compressed data, was "tkintertools-2.6.2.tar", last modified: Tue May 30 05:03:42 2023, max compression
```

## Comparing `tkintertools-2.6.1.2.tar` & `tkintertools-2.6.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 14:07:59.974072 tkintertools-2.6.1.2/
--rw-rw-rw-   0        0        0     7548 2023-05-20 23:03:00.000000 tkintertools-2.6.1.2/LICENSE
--rw-rw-rw-   0        0        0    26354 2023-05-22 14:07:59.973072 tkintertools-2.6.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    25847 2023-05-21 10:18:49.000000 tkintertools-2.6.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 14:07:59.974072 tkintertools-2.6.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1208 2023-05-22 14:07:49.000000 tkintertools-2.6.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:07:59.965072 tkintertools-2.6.1.2/tkintertools/
--rw-rw-rw-   0        0        0     1877 2023-05-20 20:35:35.000000 tkintertools-2.6.1.2/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    60774 2023-05-22 14:06:41.000000 tkintertools-2.6.1.2/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     1295 2023-05-22 14:06:44.000000 tkintertools-2.6.1.2/tkintertools/constants.py
--rw-rw-rw-   0        0        0      870 2023-05-14 13:27:34.000000 tkintertools-2.6.1.2/tkintertools/md.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:07:59.971075 tkintertools-2.6.1.2/tkintertools.egg-info/
--rw-rw-rw-   0        0        0    26354 2023-05-22 14:07:59.000000 tkintertools-2.6.1.2/tkintertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-22 14:07:59.000000 tkintertools-2.6.1.2/tkintertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 14:07:59.000000 tkintertools-2.6.1.2/tkintertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-22 14:07:59.000000 tkintertools-2.6.1.2/tkintertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 05:03:42.315983 tkintertools-2.6.2/
+-rw-rw-rw-   0        0        0     7548 2023-05-27 20:59:02.000000 tkintertools-2.6.2/LICENSE
+-rw-rw-rw-   0        0        0    28242 2023-05-30 05:03:42.314979 tkintertools-2.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0    27737 2023-05-30 05:02:43.000000 tkintertools-2.6.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-30 05:03:42.315983 tkintertools-2.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1206 2023-05-30 05:00:07.000000 tkintertools-2.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:03:42.307980 tkintertools-2.6.2/tkintertools/
+-rw-rw-rw-   0        0        0     1852 2023-05-29 13:41:50.000000 tkintertools-2.6.2/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    60774 2023-05-29 12:50:33.000000 tkintertools-2.6.2/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     1359 2023-05-29 16:01:56.000000 tkintertools-2.6.2/tkintertools/constants.py
+-rw-rw-rw-   0        0        0    14044 2023-05-30 03:03:47.000000 tkintertools-2.6.2/tkintertools/tools_3d.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:03:42.312981 tkintertools-2.6.2/tkintertools.egg-info/
+-rw-rw-rw-   0        0        0    28242 2023-05-30 05:03:42.000000 tkintertools-2.6.2/tkintertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-05-30 05:03:42.000000 tkintertools-2.6.2/tkintertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 05:03:42.000000 tkintertools-2.6.2/tkintertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-30 05:03:42.000000 tkintertools-2.6.2/tkintertools.egg-info/top_level.txt
```

### Comparing `tkintertools-2.6.1.2/LICENSE` & `tkintertools-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.1.2/PKG-INFO` & `tkintertools-2.6.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,26 @@
-Metadata-Version: 2.1
-Name: tkintertools
-Version: 2.6.1.2
-Summary: An auxiliary module of the tkinder module
-Home-page: https://gitcode.net/weixin_62651706/tkintertools
-Author: Xiaokang2022
-Author-email: 2951256653@qq.com
-License: MulanPSL-2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
     <p><img height="120px" alt="logo.png"
         src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/tkintertools.png" />
     </p>
     <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
     <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
     <p>
         <a href="./tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.1-blue" alt="latest version" />
+            <img src="https://img.shields.io/badge/Version-2.6.2-blue" alt="latest version" />
         </a>
         <a href="./LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
         <a href="./CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/05/21-orange" alt="ChangeLog" />
+            <img src="https://img.shields.io/badge/ChangeLog-2023/05/30-orange" alt="ChangeLog" />
         </a>
         <a href="./TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-10-yellow" alt="ToDos" />
+            <img src="https://img.shields.io/badge/ToDos-13-yellow" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
             <img src="https://img.shields.io/badge/Downloads-3k-purple" alt="Downloads" />
         </a>
     </p>
     <p>
         <a href="mailto:2951256653@qq.com">
@@ -50,40 +36,149 @@
 </div>
 
 Installation/模块安装
 -----------------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.1
-* Release Date/发布日期 : 2023/05/21
+* Version/版本 : 2.6.2
+* Release Date/发布日期 : 2023/05/30
 
 ```
-pip install tkintertools==2.6.1
+pip install tkintertools==2.6.2
 ```
 或者
 ```
 pip install tkintertools
 ```
 
-这个是目前的最新版，比较稳定，bug 没有那么多，推荐使用这个。  
+这个是目前的最新稳定版，比较稳定，bug 没有那么多，推荐使用这个。  
 稳定版有文档可以查看，有 issue 我会去查看并尝试解决 issue。
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.1
-* Release Date/发布日期 : 2023/05/21
+* Version/版本 : 2.6.2
+* Release Date/发布日期 : 2023/05/26
 
 ```
-pip install tkintertools-dev==2.6.1
+pip install tkintertools-dev==2.6.2
 ```
 
 这个是作者正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
 开发版本没有对应的文档，大家可以在 issue 中提出建议，我会适当采纳一些并在开发版本中更改或实现。
 
+News/最新功能
+------------
+
+最新版的`tkintertools`为`2.6.2`，新增一项极为强大的功能：3d绘图！  
+同时修复一些bug，优化了一部分代码，提升了一部分性能。
+
+通过以下代码来使用3d绘图功能：
+
+```python
+from tkintertools import tools_3d as t3d
+import tkintertools.tools_3d as t3d
+# 两种引入方式都可以
+```
+
+子模块: [tools_3d.py](./tkintertools/tools_3d.py)
+
+目前3d绘图功能还比较简陋，仅能绘制点、线、面以及直边的空间几何体，对于曲边的空间几何体还在开发中！  
+以下是一个使用3d绘图的示例：
+
+在这个示例中，按住鼠标左键可以旋转几何体，按住鼠标右键可以平移几何体，滚动鼠标滚轮可以缩放几何体！  
+x、y 和 z 轴分别是红色、绿色和蓝色的线。
+
+![3d绘图](./docs/images/3d.png)
+
+<details><summary><b>源代码</b></summary>
+
+```python
+import random
+import tkinter
+
+import tkintertools as tkt
+from tkintertools import tools_3d as t3d
+
+root = tkt.Tk('tools_3d', 1280, 720)
+canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0)
+
+geos = []  # type: list[t3d.Geometry]
+origin = t3d.Point(canvas, [0, 0, 0], size=5)  # 原点
+axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'),  # 创建坐标轴
+        t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3, fill='green'),
+        t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
+
+for _ in range(8):
+    # 创建正方体
+    cube = t3d.Cuboid(
+        canvas, *random.sample(range(-200, 200), 3), *random.sample(range(50, 100), 3))
+    geos.append(cube)
+    # 创建四面体
+    x, y, z = random.sample(range(-200, 200), 3)
+    tetr = t3d.Tetrahedron(
+        canvas, *[[x+random.randint(-100, 100), y+random.randint(-100, 100), z+random.randint(-100, 100)] for _ in range(4)])
+    geos.append(tetr)
+
+
+def translate(event, flag=False, _cache=[]):
+    # type: (tkinter.Event, bool, list[float]) -> None
+    """ 平移事件 """
+    if flag:
+        _cache[:] = [event.x, event.y]
+        return
+    dx = (event.x - _cache[0]) / 6
+    dy = (event.y - _cache[1]) / 6
+    _cache[:] = [event.x, event.y]
+    for axis in axes:
+        axis.translate(0, 6*dx, 6*dy)
+        axis.update()
+    for geo in geos:
+        geo.translate(0, dx, dy)
+        geo.update()
+    origin.translate(0, 6*dx, 6*dy)
+    origin.update()
+
+
+def rotate(event, flag=False, _cache=[]):  # type: (tkinter.Event, bool, list[float]) -> None
+    """ 旋转事件 """
+    if flag:
+        _cache[:] = [event.x, event.y]
+        return
+    dy = (event.x - _cache[0]) / 200
+    dx = (_cache[1] - event.y) / 200
+    _cache[:] = [event.x, event.y]
+    for axis in axes:
+        axis.rotate(0, 6*dx, 6*dy, center=origin.coords)
+        axis.update()
+    for geo in geos:
+        geo.rotate(0, dx, dy, center=origin.coords)
+        geo.update()
+
+
+def scale(event):  # type: (tkinter.Event) -> None
+    """ 缩放事件 """
+    k = 1.01 if event.delta > 0 else 0.99
+    for geo in geos:
+        geo.scale(k, k, k)
+        geo.update()
+
+
+root.bind('<Button-1>', lambda event: rotate(event, True))
+root.bind('<B1-Motion>', rotate)
+root.bind('<Button-3>', lambda event: translate(event, True))
+root.bind('<B3-Motion>', translate)
+root.bind('<MouseWheel>', scale)
+root.mainloop()
+```
+
+</details>
+
+更多更新信息请见：[CHANGELOG.md](./CHANGELOG.md)
+
 Description/模块说明
 ----------------------
 
 tkintertools 是一款基于 tkinter 模块的二次开发的界面编程模块，它完全没有使用任何第三方模块和库的，同时，它也没有任何依赖包，它的功能完全由内置模块和函数实现，而且，它还是跨平台的！它和 tkinter 最大的不同在于，它的控件并非真实的控件，而是在 tkinter 模块中 Canvas 对象中绘制而成的，这就赋予了 tkintertools 控件一些在 tkinter 中没有的特性，列举如下：
 
 * 控件背景可以是透明的（实际上是没有背景颜色）
 * 控件的样式可以是自定义的（比如按钮有圆角）
@@ -134,27 +229,27 @@
 见 [DPI 级别设置函数](#DPI)
 
 ### Detailed type hints/详细的类型提示
 
 参考 [PEP 526](https://peps.python.org/pep-0526/)、[PEP 586](https://peps.python.org/pep-0586/)、[PEP 604](https://peps.python.org/pep-0604/) 和 [PEP 612](https://peps.python.org/pep-0612/)，我采用了最兼容的方式去实现详细的类型提示，可适用 IDE 有 VScode、Pycharm 等。  
 那什么是类型提示呢？话不多说，直接看图就行：
 
-<p><img height="350px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/type_hint_vscode.png" alt="type_hint.png"/></p>
+![type_hint.png](docs/images/type_hint_vscode.png)
 
 在 VSCode 编辑器中，当鼠标移至类或者函数的名字上面时，会自动显示该类或者函数的注释文档。通过这种方式，不需要看太多的帮助文档和资料就能熟练地使用 tkintertools 模块！
 
 ### Across Platforms/跨平台
 
 [test.py](./test.py) 在 Windows 系统（Windows10）上运行的界面如下：
 
-<p><img height="383px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/test_win32.png" alt="test_win32.png"/></p>
+![test_win32.png](docs/images/test_win32.png)
 
 [test.py](./test.py) 在 Linux 系统（Ubuntu22.04）上运行的界面如下：
 
-<p><img height="408px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/test_linux.png" alt="test_linux.png"/></p>
+![test_linux.png](docs/images/test_linux.png)
 
 Contents/模块内容
 -------------------
 
 Each non internal class and function in the module will be described in detail here  
 这里会详细说明模块中的每个非内部类和函数
 
@@ -174,15 +269,16 @@
 
 ### Virtual Canvas Widget/虚拟画布控件
 
 1. `Label`: 标签控件
 
     标签控件的功能和`tkinter.Label`的功能类似，但更加的多元化  
     下面是`Label`控件的外观：  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/LabelTest.png" alt="LabelTest.png" /></p>
+
+    ![LabelTest.png](docs/images/LabelTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('LabelTest', 1000, 400)
@@ -207,16 +303,17 @@
     ```
 
     </details>
 
 2. `Button`: 按钮控件
 
     按钮控件相较于`tkinter.Button`，其自由度更高，`tkinter.Button`只有在按下的时候才能触发绑定的关联事件，而`Button`却可以在鼠标移至按钮上方时、鼠标按下时、鼠标松开时都可以绑定关联事件  
-    下面是`Button`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ButtonTest.png" alt="ButtonTest.png" /></p>
+    下面是`Button`控件的外观：
+
+    ![ButtonTest.png](docs/images/ButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ButtonTest', 500, 500)
@@ -242,15 +339,16 @@
 
     </details>
 
 3. `CheckButton`: 复选框控件
 
     复选框控件相对于`tkinter`原生的`tkinter.CheckButton`在使用方面更加地简单，同时颜值也上升了不少  
     下面是`CheckButton`控件的外观：
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/CheckButtonTest.png" alt="CheckButtonTest.png"/></p>
+
+    ![CheckButtonTest.png](docs/images/CheckButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('CheckButtonTest', 500, 300)
@@ -276,16 +374,17 @@
     ```
 
     </details>
 
 4. `Entry`: 输入框控件
 
     输入框控件可以轻松地设置输入的文本位置（靠左、居中和靠右），同时，它可以在鼠标移至输入框上方、鼠标未在输入框上方两种状态显示不同的默认文本  
-    下面是`Entry`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/EntryTest.png" alt="EntryTest.png" /></p>
+    下面是`Entry`控件的外观：
+
+    ![EntryTest.png](docs/images/EntryTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('EntryTest', 500, 400)
@@ -321,16 +420,17 @@
     ```
 
     </details>
 
 5. `Text`: 文本框控件
 
     文本框类似于输入框，这里就不再赘述  
-    下面是`Text`控件的外观：  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/TextTest.png" alt="TextTest.png" /></p>
+    下面是`Text`控件的外观：
+
+    ![TextTest.png](docs/images/TextTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('TextTest', 1000, 400)
@@ -356,16 +456,17 @@
     ```
 
     </details>
 
 6. `Progressbar`: 进度条控件
 
     进度条控件相比`tkinter.ttk.Progressbar`，外观上的自由度较大  
-    下面是`Progressbar`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ProgressbarTest.png" alt="ProgressbarTest.png" /></p>
+    下面是`Progressbar`控件的外观：
+
+    ![ProgressbarTest.png](docs/images/ProgressbarTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ProgressbarTest', 500, 500)
@@ -417,16 +518,17 @@
 
     单例模式，不用介绍了吧？通过继承它来使用
 
 ### Tool Function/工具函数
 
 1. `move`: <a name="move">移动函数</a>
 
-    移动函数可以轻松地按一定的规律、移动速度、移动时间去移动`tkintertools`模块内的所有对象，同时兼容了`tkinter`内的对象，即`tkinter`中的对象也可以很方便地移动，甚至它还可以移动窗口的位置！  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/MoveTest.gif" alt="MoveTest.gif" /></p>
+    移动函数可以轻松地按一定的规律、移动速度、移动时间去移动`tkintertools`模块内的所有对象，同时兼容了`tkinter`内的对象，即`tkinter`中的对象也可以很方便地移动，甚至它还可以移动窗口的位置！
+
+    ![MoveTest.gif](docs/images/MoveTest.gif)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('MoveTest', 500, 500)
@@ -470,17 +572,19 @@
     `left`   : "tkintertools        "  
     `center` : "    tkintertools    "  
     `right`  : "        tkintertools"</pre>
 
 3. `color`: <a name="Gradient">颜色函数</a>
 
     颜色函数可以轻松求出一个颜色到另外一个颜色的过渡颜色，因此可以轻松得到渐变色的效果，同时，改变传入的参数还可以得到传入颜色的对比色  
-    第二张图是 test.py 在图像测试中绘制的图案  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ColorTest.png" alt="ColorTest.png" />
-    <img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/Test_Draw.png" alt="Test_Draw.png" /></p>
+    第二张图是 test.py 在图像测试中绘制的图案
+
+    ![ColorTest.png](docs/images/ColorTest.png)
+
+    ![Test_Draw.png](docs/images/Test_Draw.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ColorTest', 500, 500)
@@ -510,19 +614,19 @@
     <p><img width="540px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/font.png" alt="font.png" /></p>
 
 5. `SetProcessDpiAwareness`: <a name="DPI">DPI 级别设置函数</a>
 
     这个函数实际上只是对函数`ctypes.WinDLL('shcore').SetProcessDpiAwareness`的一个简单包装，其值可为 0、1 和 2，分别代表程序 DPI 的不同级别，那么缩放效果也就不同，`tkintertools`选择的值是 1，但程序默认值实际为 0  
     下面是未执行这个函数的效果
     
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/SetProcessDpiAwareness_0.png" alt="SetProcessDpiAwareness_0.png" /></p>
+    ![SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
 
     <p>下面是执行了这个函数的效果</p>
 
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/SetProcessDpiAwareness_1.png" alt="SetProcessDpiAwareness_1.png" /></p>
+    ![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
 
     从上面的两张图中可以很明显的看出第一张很模糊，第二张很清晰，这就是 DPI 级别不同的原因，不过这一点在屏幕缩放比不是 100% 的时候才会出现  
     大家对上面的图肯定很熟悉，这不就是 IDLE 吗！？对，这个的问题的解决办法也是来自于 IDLE 的源代码 [pyshell.py line 18~20]  
     注意：该函数在程序的不同位置执行的效果不一样！一般用在`mainloop`之前，但`tkintertools`已经在`mainloop`函数中嵌入了该函数，无需再设置一次 DPI 级别，此函数是为了原生`tkinter`程序用的。
 
 Examples/实战示例
 ----------------
@@ -565,25 +669,23 @@
 * 文章链接: 暂无
 * 代码仓库: https://gitcode.net/weixin_62651706/tester
 * 程序下载: 暂无
 * 推荐指数: 👍👍👍
 
 这个案例使用了最新稳定版的 tkintertools-v2.6.0，界面非常稳定，几乎没有 bug，完全采用 tkintertools 的控件，颜值很高，界面非常流畅。体现了 tkintertools 模块与 tkinter 模块相比在性能上的优越性！
 
-<p>
-    <img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/examples/exam3_1.png" alt="client.png"/>
-    <img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/examples/exam3_2.png" alt="client.png"/>
-</p>
+![exam3_1.png](docs/examples/exam3_1.png)
+![exam3_2.png](docs/examples/exam3_2.png)
 
 More/更多
 ---------
 
-> GitCode:  
-> https://gitcode.net/weixin_62651706/tkintertools
+> GitHub:  
+> https://github.com/Xiaokang2022/tkintertools
 
-> GitHub(Mirror/镜像):  
-> https://github.com/XiaoKang2022-CSDN/tkintertools
+> GitCode(Mirror/镜像):  
+> https://gitcode.net/weixin_62651706/tkintertools
 
-> Column/专栏:  
-> https://blog.csdn.net/weixin_62651706/category_11600888.html
+> Gitee(Mirror/镜像):  
+> https://gitee.com/xiaokang-2022/tkintertools
 
 还有更多内容请在 [源代码](./tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,33 +1,66 @@
-Metadata-Version: 2.1 Name: tkintertools Version: 2.6.1.2 Summary: An auxiliary
-module of the tkinder module Home-page: https://gitcode.net/weixin_62651706/
-tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com License:
-MulanPSL-2.0 Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
-Classifier: Operating System :: OS Independent Description-Content-Type: text/
-markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
                             [Email] [Blog] [Author]
 Installation/æ¨¡åå®è£ ----------------------- ### Stable version/
-ç¨³å®çæ¬ * Version/çæ¬ : 2.6.1 * Release Date/åå¸æ¥æ : 2023/05/21
-``` pip install tkintertools==2.6.1 ``` æè ``` pip install tkintertools ```
-è¿ä¸ªæ¯ç®åçææ°çï¼æ¯è¾ç¨³å®ï¼bug
+ç¨³å®çæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/30
+``` pip install tkintertools==2.6.2 ``` æè ``` pip install tkintertools ```
+è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
 æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã ç¨³å®çæææ¡£å¯ä»¥æ¥çï¼æ
 issue æä¼å»æ¥çå¹¶å°è¯è§£å³ issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.1 * Release Date/åå¸æ¥æ : 2023/05/21
-``` pip install tkintertools-dev==2.6.1 ```
+å¼åçæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/26
+``` pip install tkintertools-dev==2.6.2 ```
 è¿ä¸ªæ¯ä½èæ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
 å¯è½ä¼æ¯è¾å¤ã å¼åçæ¬æ²¡æå¯¹åºçææ¡£ï¼å¤§å®¶å¯ä»¥å¨ issue
 ä¸­æåºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
-Description/æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº
-tkinter
+News/ææ°åè½ -----------
+-
+ææ°çç`tkintertools`ä¸º`2.6.2`ï¼æ°å¢ä¸é¡¹æä¸ºå¼ºå¤§çåè½ï¼3dç»å¾ï¼
+åæ¶ä¿®å¤ä¸äºbugï¼ä¼åäºä¸é¨åä»£ç ï¼æåäºä¸é¨åæ§è½ã
+éè¿ä»¥ä¸ä»£ç æ¥ä½¿ç¨3dç»å¾åè½ï¼ ```python from tkintertools import
+tools_3d as t3d import tkintertools.tools_3d as t3d #
+ä¸¤ç§å¼å¥æ¹å¼é½å¯ä»¥ ``` å­æ¨¡å: [tools_3d.py](./tkintertools/
+tools_3d.py)
+ç®å3dç»å¾åè½è¿æ¯è¾ç®éï¼ä»è½ç»å¶ç¹ãçº¿ãé¢ä»¥åç´è¾¹çç©ºé´å ä½ä½ï¼å¯¹äºæ²è¾¹çç©ºé´å ä½ä½è¿å¨å¼åä¸­ï¼
+ä»¥ä¸æ¯ä¸ä¸ªä½¿ç¨3dç»å¾çç¤ºä¾ï¼
+å¨è¿ä¸ªç¤ºä¾ä¸­ï¼æä½é¼ æ å·¦é®å¯ä»¥æè½¬å ä½ä½ï¼æä½é¼ æ å³é®å¯ä»¥å¹³ç§»å ä½ä½ï¼æ»å¨é¼ æ æ»è½®å¯ä»¥ç¼©æ¾å ä½ä½ï¼
+xãy å z è½´åå«æ¯çº¢è²ãç»¿è²åèè²ççº¿ã ![3dç»å¾](./docs/
+images/3d.png) æºä»£ç  ```python import random import tkinter import
+tkintertools as tkt from tkintertools import tools_3d as t3d root = tkt.Tk
+('tools_3d', 1280, 720) canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0) geos = []
+# type: list[t3d.Geometry] origin = t3d.Point(canvas, [0, 0, 0], size=5) #
+åç¹ axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'), #
+åå»ºåæ è½´ t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3,
+fill='green'), t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
+for _ in range(8): # åå»ºæ­£æ¹ä½ cube = t3d.Cuboid( canvas, *random.sample
+(range(-200, 200), 3), *random.sample(range(50, 100), 3)) geos.append(cube) #
+åå»ºåé¢ä½ x, y, z = random.sample(range(-200, 200), 3) tetr =
+t3d.Tetrahedron( canvas, *[[x+random.randint(-100, 100), y+random.randint(-100,
+100), z+random.randint(-100, 100)] for _ in range(4)]) geos.append(tetr) def
+translate(event, flag=False, _cache=[]): # type: (tkinter.Event, bool, list
+[float]) -> None """ å¹³ç§»äºä»¶ """ if flag: _cache[:] = [event.x, event.y]
+return dx = (event.x - _cache[0]) / 6 dy = (event.y - _cache[1]) / 6 _cache[:
+] = [event.x, event.y] for axis in axes: axis.translate(0, 6*dx, 6*dy)
+axis.update() for geo in geos: geo.translate(0, dx, dy) geo.update()
+origin.translate(0, 6*dx, 6*dy) origin.update() def rotate(event, flag=False,
+_cache=[]): # type: (tkinter.Event, bool, list[float]) -> None """ æè½¬äºä»¶
+""" if flag: _cache[:] = [event.x, event.y] return dy = (event.x - _cache[0]) /
+200 dx = (_cache[1] - event.y) / 200 _cache[:] = [event.x, event.y] for axis in
+axes: axis.rotate(0, 6*dx, 6*dy, center=origin.coords) axis.update() for geo in
+geos: geo.rotate(0, dx, dy, center=origin.coords) geo.update() def scale
+(event): # type: (tkinter.Event) -> None """ ç¼©æ¾äºä»¶ """ k = 1.01 if
+event.delta > 0 else 0.99 for geo in geos: geo.scale(k, k, k) geo.update()
+root.bind('', lambda event: rotate(event, True)) root.bind('', rotate)
+root.bind('', lambda event: translate(event, True)) root.bind('', translate)
+root.bind('', scale) root.mainloop() ```  æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼
+[CHANGELOG.md](./CHANGELOG.md) Description/æ¨¡åè¯´æ ---------------------
+- tkintertools æ¯ä¸æ¬¾åºäº tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
 tkinter æ¨¡åä¸­ Canvas å¯¹è±¡ä¸­ç»å¶èæçï¼è¿å°±èµäºäº
 tkintertools æ§ä»¶ä¸äºå¨ tkinter ä¸­æ²¡æçç¹æ§ï¼åä¸¾å¦ä¸ï¼ *
 æ§ä»¶èæ¯å¯ä»¥æ¯éæçï¼å®éä¸æ¯æ²¡æèæ¯é¢è²ï¼ *
 æ§ä»¶çæ ·å¼å¯ä»¥æ¯èªå®ä¹çï¼æ¯å¦æé®æåè§ï¼ *
 æ§ä»¶çåå»ºéåº¦è¿å¤§äº tkinter çæ§ä»¶ï¼é¤äº Canvas æ§ä»¶ï¼
@@ -58,78 +91,71 @@
 (#Gradient) ### Automatically adapt to DPI/èªå¨éåºDPI è§ [DPI
 çº§å«è®¾ç½®å½æ°](#DPI) ### Detailed type hints/è¯¦ç»çç±»åæç¤º åè
 [PEP 526](https://peps.python.org/pep-0526/)ã[PEP 586](https://
 peps.python.org/pep-0586/)ã[PEP 604](https://peps.python.org/pep-0604/) å
 [PEP 612](https://peps.python.org/pep-0612/
 )ï¼æéç¨äºæå¼å®¹çæ¹å¼å»å®ç°è¯¦ç»çç±»åæç¤ºï¼å¯éç¨
 IDE æ VScodeãPycharm ç­ã
-é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼
-[type_hint.png]
-å¨ VSCode
+é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼ !
+[type_hint.png](docs/images/type_hint_vscode.png) å¨ VSCode
 ç¼è¾å¨ä¸­ï¼å½é¼ æ ç§»è³ç±»æèå½æ°çåå­ä¸é¢æ¶ï¼ä¼èªå¨æ¾ç¤ºè¯¥ç±»æèå½æ°çæ³¨éææ¡£ãéè¿è¿ç§æ¹å¼ï¼ä¸éè¦çå¤ªå¤çå¸®å©ææ¡£åèµæå°±è½çç»å°ä½¿ç¨
 tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](./test.py) å¨
-Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼
-[test_win32.png]
-[test.py](./test.py) å¨ Linux
-ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼
-[test_linux.png]
-Contents/æ¨¡ååå®¹ ------------------- Each non internal class and function
-in the module will be described in detail here
+Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_win32.png]
+(docs/images/test_win32.png) [test.py](./test.py) å¨ Linux
+ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png](docs/
+images/test_linux.png) Contents/æ¨¡ååå®¹ ------------------- Each non
+internal class and function in the module will be described in detail here
 è¿éä¼è¯¦ç»è¯´ææ¨¡åä¸­çæ¯ä¸ªéåé¨ç±»åå½æ° ### Container
 Widget/å®¹å¨æ§ä»¶ 1. `Tk`: çªå£ç±»
 ç»§æ¿äº`tkinter.Tk`ï¼å¨ç»§æ¿äº`tkinter`æ¨¡åå`Tk`çåºç¡ä¸ï¼åå å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¹¶å å¥äºæ£æµçªå£å¤§å°æ¯å¦ç¼©æ¾çæºå¶ï¼ä»¥ä½¿å¾å¶å­`Canvas`åè½æ­£ç¡®å°è¿è¡ç¼©æ¾
 2. `Toplevel`: é¡¶çº§çªå£ç±»
 ç»§æ¿äº`tkinter.Toplevel`å`Tk`ï¼å å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¶ä½åä¸`Tk`ä¸æ ·
 3. `Canvas`: ç»å¸ç±»
 ç»§æ¿äº`tkinter.Canvas`ï¼å å¥äºå¯¹ç»å¸èææ§ä»¶çæ¯æï¼åæ¶æ¯åç±»ååºäºä»¶ãç¼©æ¾æ§å¶çç®¡çèï¼ä¹å¯¹`tkinter.Canvas`çå®ä¾æ¹æ³æä¸å®çå¼å®¹æ§
 ### Virtual Canvas Widget/èæç»å¸æ§ä»¶ 1. `Label`: æ ç­¾æ§ä»¶
 æ ç­¾æ§ä»¶çåè½å`tkinter.Label`çåè½ç±»ä¼¼ï¼ä½æ´å çå¤åå
-ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼
-[LabelTest.png]
+ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼ ![LabelTest.png](docs/images/LabelTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('LabelTest', 1000,
 400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Label(canvas, 50, 50, 400, 100, text='NormalLabel\nHere is the text')
 tkt.Label(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerLabel')
 tkt.Label(canvas, 550, 50, 400, 100, text='DisableLabel').set_live(False)
 tkt.Label(canvas, 550, 200, 400, 100, radius=20, text='TransparentLabel',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  2. `Button`: æé®æ§ä»¶
 æé®æ§ä»¶ç¸è¾äº`tkinter.Button`ï¼å¶èªç±åº¦æ´é«ï¼`tkinter.Button`åªæå¨æä¸çæ¶åæè½è§¦åç»å®çå³èäºä»¶ï¼è`Button`å´å¯ä»¥å¨é¼ æ ç§»è³æé®ä¸æ¹æ¶ãé¼ æ æä¸æ¶ãé¼ æ æ¾å¼æ¶é½å¯ä»¥ç»å®å³èäºä»¶
-ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼
-[ButtonTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ButtonTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
-height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
-range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼ ![ButtonTest.png](docs/images/
+ButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk
+('ButtonTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful
+(x, y, width, height): # type: (int, int, int, int) -> None """ Gradient colors
+""" for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 280, 400,
 100) tkt.Button(canvas, 150, 135, 200, 50, text='NormalButton') tkt.Button
 (canvas, 100, 195, 300, 50, radius=10, text='RoundCornerButton') tkt.Button
 (canvas, 150, 255, 200, 50, text='DisableButton').set_live(False) tkt.Button
 (canvas, 100, 315, 300, 50, radius=10, text='TransparentButton',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  3. `CheckButton`:
 å¤éæ¡æ§ä»¶
 å¤éæ¡æ§ä»¶ç¸å¯¹äº`tkinter`åçç`tkinter.CheckButton`å¨ä½¿ç¨æ¹é¢æ´å å°ç®åï¼åæ¶é¢å¼ä¹ä¸åäºä¸å°
-ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼
-[CheckButtonTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('CheckButtonTest',
-500, 300) canvas = tkt.Canvas(root, 500, 300, 0, 0) def colorful(x, y, width,
-height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
-range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
-canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(40, 190, 420,
-50) tkt.CheckButton(canvas, 50, 50, 30, text='NormalCheckButton', value=True)
-tkt.CheckButton(canvas, 50, 100, 30, text='DisableCheckButton',
-value=True).set_live(False) tkt.CheckButton(canvas, 50, 150, 30, radius=10,
-text='RoundCornerCheckButton') tkt.CheckButton(canvas, 50, 200, 30, radius=15,
-text='TransparentCheckButton', color_fill=tkt.COLOR_NONE) root.mainloop() ```
-4. `Entry`: è¾å¥æ¡æ§ä»¶
+ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼ ![CheckButtonTest.png](docs/images/
+CheckButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root =
+tkt.Tk('CheckButtonTest', 500, 300) canvas = tkt.Canvas(root, 500, 300, 0, 0)
+def colorful(x, y, width, height): # type: (int, int, int, int) -> None """
+Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
+'#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
+colorful(40, 190, 420, 50) tkt.CheckButton(canvas, 50, 50, 30,
+text='NormalCheckButton', value=True) tkt.CheckButton(canvas, 50, 100, 30,
+text='DisableCheckButton', value=True).set_live(False) tkt.CheckButton(canvas,
+50, 150, 30, radius=10, text='RoundCornerCheckButton') tkt.CheckButton(canvas,
+50, 200, 30, radius=15, text='TransparentCheckButton',
+color_fill=tkt.COLOR_NONE) root.mainloop() ```  4. `Entry`: è¾å¥æ¡æ§ä»¶
 è¾å¥æ¡æ§ä»¶å¯ä»¥è½»æ¾å°è®¾ç½®è¾å¥çææ¬ä½ç½®ï¼é å·¦ãå±ä¸­åé å³ï¼ï¼åæ¶ï¼å®å¯ä»¥å¨é¼ æ ç§»è³è¾å¥æ¡ä¸æ¹ãé¼ æ æªå¨è¾å¥æ¡ä¸æ¹ä¸¤ç§ç¶ææ¾ç¤ºä¸åçé»è®¤ææ¬
-ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼
-[EntryTest.png]
+ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼ ![EntryTest.png](docs/images/EntryTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('EntryTest', 500,
 400) canvas = tkt.Canvas(root, 500, 400, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 193, 400,
 100) tkt.Entry(canvas, 20, 20, 200, 30, text=('LeftEntry', 'Enter')) tkt.Entry
 (canvas, 20, 55, 200, 30, text=( 'CenterEntry', 'Enter'), justify='center')
@@ -140,79 +166,77 @@
 radius=8, text='RightEntry', justify='right') tkt.Entry(canvas, 100, 150, 300,
 35, text=('PasswordEntry', 'Click To Enter'), justify='center', show='â')
 tkt.Entry(canvas, 100, 200, 300, 35, text='DisableEntry',
 justify='center').set_live(False) tkt.Entry(canvas, 100, 250, 300, 35,
 text='TransparentEntry', justify='center', color_fill=tkt.COLOR_NONE)
 root.mainloop() ```  5. `Text`: ææ¬æ¡æ§ä»¶
 ææ¬æ¡ç±»ä¼¼äºè¾å¥æ¡ï¼è¿éå°±ä¸åèµè¿°
-ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼
-[TextTest.png]
+ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼ ![TextTest.png](docs/images/TextTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('TextTest', 1000,
 400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
 height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
 for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Text(canvas, 50, 50, 400, 100, text=('NormalText(Left)', 'Click To
 Enter')) tkt.Text(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerText
 (Center)', justify='center') tkt.Text(canvas, 550, 50, 400, 100,
 text='DisableText').set_live(False) tkt.Text(canvas, 550, 200, 400, 100,
 radius=20, text='TransparentText(Right)', justify='right',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  6. `Progressbar`:
 è¿åº¦æ¡æ§ä»¶
 è¿åº¦æ¡æ§ä»¶ç¸æ¯`tkinter.ttk.Progressbar`ï¼å¤è§ä¸çèªç±åº¦è¾å¤§
-ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼
-[ProgressbarTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ProgressbarTest',
-500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
-height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
-for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
-canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(30, 290, 440,
-50) tkt.Progressbar(canvas, 50, 50, 400, 30) tkt.Progressbar(canvas, 50, 100,
-400, 30).load(.6667) tkt.Progressbar(canvas, 50, 150, 400, 30,
-borderwidth=5).load(1) (_ := tkt.Progressbar(canvas, 50, 200, 400, 30)).load
-(0.3333) _.set_live(False) tkt.Progressbar(canvas, 50, 250, 400, 30, color_bar=
-( 'lightyellow', 'skyblue')).load(.5) tkt.Progressbar(canvas, 50, 300, 400, 30,
-color_bar=('', 'orange')).load(.1667) progressbar = tkt.Progressbar(canvas, 50,
-375, 400, 30) progressbar_2 = tkt.Progressbar(canvas, 50, 425, 400, 30) def
-load(total, count=0): # type: (int, int) -> None """ load progressbar """
-progressbar.load(count/total) progressbar_2.load(1-count/total) if count <
-total: root.after(3, load, total, count+1) load(10000) root.mainloop() ```  ###
-Tool Class/å·¥å·ç±» 1. `PhotoImage`: å¾çç±»
+ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼ ![ProgressbarTest.png](docs/images/
+ProgressbarTest.png) æºä»£ç  ```python import tkintertools as tkt root =
+tkt.Tk('ProgressbarTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0)
+def colorful(x, y, width, height) -> None: # type: (int, int, int, int) -> None
+""" Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
+'#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
+colorful(30, 290, 440, 50) tkt.Progressbar(canvas, 50, 50, 400, 30)
+tkt.Progressbar(canvas, 50, 100, 400, 30).load(.6667) tkt.Progressbar(canvas,
+50, 150, 400, 30, borderwidth=5).load(1) (_ := tkt.Progressbar(canvas, 50, 200,
+400, 30)).load(0.3333) _.set_live(False) tkt.Progressbar(canvas, 50, 250, 400,
+30, color_bar=( 'lightyellow', 'skyblue')).load(.5) tkt.Progressbar(canvas, 50,
+300, 400, 30, color_bar=('', 'orange')).load(.1667) progressbar =
+tkt.Progressbar(canvas, 50, 375, 400, 30) progressbar_2 = tkt.Progressbar
+(canvas, 50, 425, 400, 30) def load(total, count=0): # type: (int, int) -> None
+""" load progressbar """ progressbar.load(count/total) progressbar_2.load(1-
+count/total) if count < total: root.after(3, load, total, count+1) load(10000)
+root.mainloop() ```  ### Tool Class/å·¥å·ç±» 1. `PhotoImage`: å¾çç±»
 `PhotoImage`ç±»ç»§æ¿äº`tkinter.PhotoImage`ï¼å®æ¯å¨`tkinter.PhotoImage`çåºç¡ä¸ååè½çå¼ºåï¼å¯¹
 gif
 å¨å¾æå¾å¥½çæ¯æï¼ä»éæå°éä»£ç å³å¯å®ç°å¨å¾çæ¾ç¤ºï¼è¿å¯ä»¥è®¾ç½®å¨å¾æ¾ç¤ºçéåº¦ï¼æ­¤å¤ï¼å¯¹
 png
 ç±»åçå¾ççæ¯æä¹æå¼ºåï¼å¯ä»¥å¨ä¸ä¾èµä»»ä½ç¬¬ä¸æ¹æ¨¡åæèåºçæåµä¸ï¼å¯¹
 png å¾çè¿è¡ç¼©æ¾ 2. `Singleton`: åä¾æ¨¡å¼ç±»
 åä¾æ¨¡å¼ï¼ä¸ç¨ä»ç»äºå§ï¼éè¿ç»§æ¿å®æ¥ä½¿ç¨ ### Tool Function/
 å·¥å·å½æ° 1. `move`: ç§»å¨å½æ°
 ç§»å¨å½æ°å¯ä»¥è½»æ¾å°æä¸å®çè§å¾ãç§»å¨éåº¦ãç§»å¨æ¶é´å»ç§»å¨`tkintertools`æ¨¡ååçææå¯¹è±¡ï¼åæ¶å¼å®¹äº`tkinter`åçå¯¹è±¡ï¼å³`tkinter`ä¸­çå¯¹è±¡ä¹å¯ä»¥å¾æ¹ä¾¿å°ç§»å¨ï¼çè³å®è¿å¯ä»¥ç§»å¨çªå£çä½ç½®ï¼
-[MoveTest.gif]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('MoveTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500, 0, 0) rect = canvas.create_rectangle
-(50, 350, 150, 450) def move_window(switch=[True]): # type: (list[bool]) -
-> None tkt.move(root, None, 1000 if switch[0] else -1000, 0, 800, mode='flat')
-switch[0] = not switch[0] def move_button(switch=[True]) -> None: # type: (list
-[bool]) -> None tkt.move(canvas, button, 200 if switch[0] else -200, 0, 500,
-mode='rebound') switch[0] = not switch[0] def move_rect(switch=[True]): # type:
-(list[bool]) -> None tkt.move(canvas, rect, 200 if switch[0] else -200, 0, 500,
-mode='smooth') switch[0] = not switch[0] tkt.Button(canvas, 50, 50, 200, 40,
-radius=10, text='MoveWindow', command=move_window) tkt.Button(canvas, 50, 100,
-200, 40, radius=10, text='MoveRect', command=move_rect) button = tkt.Button
-(canvas, 50, 150, 200, 40, radius=10, text='MoveButton', command=move_button)
-root.mainloop() ```  2. `text`: ææ¬å½æ°
+![MoveTest.gif](docs/images/MoveTest.gif) æºä»£ç  ```python import
+tkintertools as tkt root = tkt.Tk('MoveTest', 500, 500) canvas = tkt.Canvas
+(root, 500, 500, 0, 0) rect = canvas.create_rectangle(50, 350, 150, 450) def
+move_window(switch=[True]): # type: (list[bool]) -> None tkt.move(root, None,
+1000 if switch[0] else -1000, 0, 800, mode='flat') switch[0] = not switch[0]
+def move_button(switch=[True]) -> None: # type: (list[bool]) -> None tkt.move
+(canvas, button, 200 if switch[0] else -200, 0, 500, mode='rebound') switch[0]
+= not switch[0] def move_rect(switch=[True]): # type: (list[bool]) -> None
+tkt.move(canvas, rect, 200 if switch[0] else -200, 0, 500, mode='smooth')
+switch[0] = not switch[0] tkt.Button(canvas, 50, 50, 200, 40, radius=10,
+text='MoveWindow', command=move_window) tkt.Button(canvas, 50, 100, 200, 40,
+radius=10, text='MoveRect', command=move_rect) button = tkt.Button(canvas, 50,
+150, 200, 40, radius=10, text='MoveButton', command=move_button) root.mainloop
+() ```  2. `text`: ææ¬å½æ°
 å¯ä»¥å¿«éå¹¶æ¹ä¾¿å°å¾å°ä¸ä¸ªåæ°é¿åº¦çå­ç¬¦ä¸²ï¼ä¸å­ç¬¦ä¸²çåå®¹å¯ä»¥æå®ä½ç½®
 å¦ï¼å¾å°ä¸ä¸ª 20 é¿åº¦çå­ç¬¦ä¸² âtkintertoolsâ
     `left`   : "tkintertools        "
     `center` : "    tkintertools    "
     `right`  : "        tkintertools"
 3. `color`: é¢è²å½æ°
 é¢è²å½æ°å¯ä»¥è½»æ¾æ±åºä¸ä¸ªé¢è²å°å¦å¤ä¸ä¸ªé¢è²çè¿æ¸¡é¢è²ï¼å æ­¤å¯ä»¥è½»æ¾å¾å°æ¸åè²çææï¼åæ¶ï¼æ¹åä¼ å¥çåæ°è¿å¯ä»¥å¾å°ä¼ å¥é¢è²çå¯¹æ¯è²
-ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡
-[ColorTest.png] [Test_Draw.png]
+ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡ ![ColorTest.png]
+(docs/images/ColorTest.png) ![Test_Draw.png](docs/images/Test_Draw.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ColorTest', 500,
 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 =
 tkt.color(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i,
 y+height, fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
 outline=color_2, width=2) colorful(50, 50, 400, 100) root.mainloop() ```  4.
@@ -222,18 +246,18 @@
 tcl çå½ä»¤ï¼ä½¿å¾å­ä½éæ©æ¡è½å¤è¢«æä»¬ä½¿ç¨ã
 [font.png]
 5. `SetProcessDpiAwareness`: DPI çº§å«è®¾ç½®å½æ°
 è¿ä¸ªå½æ°å®éä¸åªæ¯å¯¹å½æ°`ctypes.WinDLL
 ('shcore').SetProcessDpiAwareness`çä¸ä¸ªç®ååè£ï¼å¶å¼å¯ä¸º 0ã1
 å 2ï¼åå«ä»£è¡¨ç¨åº DPI
 çä¸åçº§å«ï¼é£ä¹ç¼©æ¾ææä¹å°±ä¸åï¼`tkintertools`éæ©çå¼æ¯
-1ï¼ä½ç¨åºé»è®¤å¼å®éä¸º 0 ä¸é¢æ¯æªæ§è¡è¿ä¸ªå½æ°çææ
-[SetProcessDpiAwareness_0.png]
+1ï¼ä½ç¨åºé»è®¤å¼å®éä¸º 0 ä¸é¢æ¯æªæ§è¡è¿ä¸ªå½æ°çææ !
+[SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
 ä¸é¢æ¯æ§è¡äºè¿ä¸ªå½æ°çææ
-[SetProcessDpiAwareness_1.png]
+![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
 ä»ä¸é¢çä¸¤å¼ å¾ä¸­å¯ä»¥å¾ææ¾ççåºç¬¬ä¸å¼ å¾æ¨¡ç³ï¼ç¬¬äºå¼ å¾æ¸æ°ï¼è¿å°±æ¯
 DPI çº§å«ä¸åçåå ï¼ä¸è¿è¿ä¸ç¹å¨å±å¹ç¼©æ¾æ¯ä¸æ¯ 100%
 çæ¶åæä¼åºç° å¤§å®¶å¯¹ä¸é¢çå¾è¯å®å¾çæï¼è¿ä¸å°±æ¯ IDLE
 åï¼ï¼å¯¹ï¼è¿ä¸ªçé®é¢çè§£å³åæ³ä¹æ¯æ¥èªäº IDLE çæºä»£ç 
 [pyshell.py line 18~20]
 æ³¨æï¼è¯¥å½æ°å¨ç¨åºçä¸åä½ç½®æ§è¡çææä¸ä¸æ ·ï¼ä¸è¬ç¨å¨`mainloop`ä¹åï¼ä½`tkintertools`å·²ç»å¨`mainloop`å½æ°ä¸­åµå¥äºè¯¥å½æ°ï¼æ éåè®¾ç½®ä¸æ¬¡
 DPI çº§å«ï¼æ­¤å½æ°æ¯ä¸ºäºåç`tkinter`ç¨åºç¨çã Examples/
@@ -262,14 +286,13 @@
 æ¨¡åçå¼å®¹æ§ï¼
 [chess.png] [chess.png]
 ### ç®æç»å½çé¢ * æç« é¾æ¥: ææ  * ä»£ç ä»åº: https://
 gitcode.net/weixin_62651706/tester * ç¨åºä¸è½½: ææ  * æ¨èææ°:
 ððð è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
-æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼
-[client.png] [client.png]
-More/æ´å¤ --------- > GitCode: > https://gitcode.net/weixin_62651706/
-tkintertools > GitHub(Mirror/éå): > https://github.com/XiaoKang2022-CSDN/
-tkintertools > Column/ä¸æ : > https://blog.csdn.net/weixin_62651706/
-category_11600888.html è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/
-) ä¸­æ¢ç´¢ï¼
+æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png](docs/
+examples/exam3_1.png) ![exam3_2.png](docs/examples/exam3_2.png) More/æ´å¤ ---
+------ > GitHub: > https://github.com/Xiaokang2022/tkintertools > GitCode
+(Mirror/éå): > https://gitcode.net/weixin_62651706/tkintertools > Gitee
+(Mirror/éå): > https://gitee.com/xiaokang-2022/tkintertools
+è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
```

### Comparing `tkintertools-2.6.1.2/README.md` & `tkintertools-2.6.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,40 @@
+Metadata-Version: 2.1
+Name: tkintertools
+Version: 2.6.2
+Summary: An auxiliary module of the tkinder module
+Home-page: https://gitcode.net/weixin_62651706/tkintertools
+Author: Xiaokang2022
+Author-email: 2951256653@qq.com
+License: MulanPSL-2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
     <h1>🚀tkintertools🚀</h1>
     <p><img height="120px" alt="logo.png"
         src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/tkintertools.png" />
     </p>
     <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
     <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
     <p>
         <a href="./tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.1-blue" alt="latest version" />
+            <img src="https://img.shields.io/badge/Version-2.6.2-blue" alt="latest version" />
         </a>
         <a href="./LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
         <a href="./CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/05/21-orange" alt="ChangeLog" />
+            <img src="https://img.shields.io/badge/ChangeLog-2023/05/30-orange" alt="ChangeLog" />
         </a>
         <a href="./TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-10-yellow" alt="ToDos" />
+            <img src="https://img.shields.io/badge/ToDos-13-yellow" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
             <img src="https://img.shields.io/badge/Downloads-3k-purple" alt="Downloads" />
         </a>
     </p>
     <p>
         <a href="mailto:2951256653@qq.com">
@@ -36,40 +50,149 @@
 </div>
 
 Installation/模块安装
 -----------------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.1
-* Release Date/发布日期 : 2023/05/21
+* Version/版本 : 2.6.2
+* Release Date/发布日期 : 2023/05/30
 
 ```
-pip install tkintertools==2.6.1
+pip install tkintertools==2.6.2
 ```
 或者
 ```
 pip install tkintertools
 ```
 
-这个是目前的最新版，比较稳定，bug 没有那么多，推荐使用这个。  
+这个是目前的最新稳定版，比较稳定，bug 没有那么多，推荐使用这个。  
 稳定版有文档可以查看，有 issue 我会去查看并尝试解决 issue。
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.1
-* Release Date/发布日期 : 2023/05/21
+* Version/版本 : 2.6.2
+* Release Date/发布日期 : 2023/05/26
 
 ```
-pip install tkintertools-dev==2.6.1
+pip install tkintertools-dev==2.6.2
 ```
 
 这个是作者正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
 开发版本没有对应的文档，大家可以在 issue 中提出建议，我会适当采纳一些并在开发版本中更改或实现。
 
+News/最新功能
+------------
+
+最新版的`tkintertools`为`2.6.2`，新增一项极为强大的功能：3d绘图！  
+同时修复一些bug，优化了一部分代码，提升了一部分性能。
+
+通过以下代码来使用3d绘图功能：
+
+```python
+from tkintertools import tools_3d as t3d
+import tkintertools.tools_3d as t3d
+# 两种引入方式都可以
+```
+
+子模块: [tools_3d.py](./tkintertools/tools_3d.py)
+
+目前3d绘图功能还比较简陋，仅能绘制点、线、面以及直边的空间几何体，对于曲边的空间几何体还在开发中！  
+以下是一个使用3d绘图的示例：
+
+在这个示例中，按住鼠标左键可以旋转几何体，按住鼠标右键可以平移几何体，滚动鼠标滚轮可以缩放几何体！  
+x、y 和 z 轴分别是红色、绿色和蓝色的线。
+
+![3d绘图](./docs/images/3d.png)
+
+<details><summary><b>源代码</b></summary>
+
+```python
+import random
+import tkinter
+
+import tkintertools as tkt
+from tkintertools import tools_3d as t3d
+
+root = tkt.Tk('tools_3d', 1280, 720)
+canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0)
+
+geos = []  # type: list[t3d.Geometry]
+origin = t3d.Point(canvas, [0, 0, 0], size=5)  # 原点
+axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'),  # 创建坐标轴
+        t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3, fill='green'),
+        t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
+
+for _ in range(8):
+    # 创建正方体
+    cube = t3d.Cuboid(
+        canvas, *random.sample(range(-200, 200), 3), *random.sample(range(50, 100), 3))
+    geos.append(cube)
+    # 创建四面体
+    x, y, z = random.sample(range(-200, 200), 3)
+    tetr = t3d.Tetrahedron(
+        canvas, *[[x+random.randint(-100, 100), y+random.randint(-100, 100), z+random.randint(-100, 100)] for _ in range(4)])
+    geos.append(tetr)
+
+
+def translate(event, flag=False, _cache=[]):
+    # type: (tkinter.Event, bool, list[float]) -> None
+    """ 平移事件 """
+    if flag:
+        _cache[:] = [event.x, event.y]
+        return
+    dx = (event.x - _cache[0]) / 6
+    dy = (event.y - _cache[1]) / 6
+    _cache[:] = [event.x, event.y]
+    for axis in axes:
+        axis.translate(0, 6*dx, 6*dy)
+        axis.update()
+    for geo in geos:
+        geo.translate(0, dx, dy)
+        geo.update()
+    origin.translate(0, 6*dx, 6*dy)
+    origin.update()
+
+
+def rotate(event, flag=False, _cache=[]):  # type: (tkinter.Event, bool, list[float]) -> None
+    """ 旋转事件 """
+    if flag:
+        _cache[:] = [event.x, event.y]
+        return
+    dy = (event.x - _cache[0]) / 200
+    dx = (_cache[1] - event.y) / 200
+    _cache[:] = [event.x, event.y]
+    for axis in axes:
+        axis.rotate(0, 6*dx, 6*dy, center=origin.coords)
+        axis.update()
+    for geo in geos:
+        geo.rotate(0, dx, dy, center=origin.coords)
+        geo.update()
+
+
+def scale(event):  # type: (tkinter.Event) -> None
+    """ 缩放事件 """
+    k = 1.01 if event.delta > 0 else 0.99
+    for geo in geos:
+        geo.scale(k, k, k)
+        geo.update()
+
+
+root.bind('<Button-1>', lambda event: rotate(event, True))
+root.bind('<B1-Motion>', rotate)
+root.bind('<Button-3>', lambda event: translate(event, True))
+root.bind('<B3-Motion>', translate)
+root.bind('<MouseWheel>', scale)
+root.mainloop()
+```
+
+</details>
+
+更多更新信息请见：[CHANGELOG.md](./CHANGELOG.md)
+
 Description/模块说明
 ----------------------
 
 tkintertools 是一款基于 tkinter 模块的二次开发的界面编程模块，它完全没有使用任何第三方模块和库的，同时，它也没有任何依赖包，它的功能完全由内置模块和函数实现，而且，它还是跨平台的！它和 tkinter 最大的不同在于，它的控件并非真实的控件，而是在 tkinter 模块中 Canvas 对象中绘制而成的，这就赋予了 tkintertools 控件一些在 tkinter 中没有的特性，列举如下：
 
 * 控件背景可以是透明的（实际上是没有背景颜色）
 * 控件的样式可以是自定义的（比如按钮有圆角）
@@ -120,27 +243,27 @@
 见 [DPI 级别设置函数](#DPI)
 
 ### Detailed type hints/详细的类型提示
 
 参考 [PEP 526](https://peps.python.org/pep-0526/)、[PEP 586](https://peps.python.org/pep-0586/)、[PEP 604](https://peps.python.org/pep-0604/) 和 [PEP 612](https://peps.python.org/pep-0612/)，我采用了最兼容的方式去实现详细的类型提示，可适用 IDE 有 VScode、Pycharm 等。  
 那什么是类型提示呢？话不多说，直接看图就行：
 
-<p><img height="350px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/type_hint_vscode.png" alt="type_hint.png"/></p>
+![type_hint.png](docs/images/type_hint_vscode.png)
 
 在 VSCode 编辑器中，当鼠标移至类或者函数的名字上面时，会自动显示该类或者函数的注释文档。通过这种方式，不需要看太多的帮助文档和资料就能熟练地使用 tkintertools 模块！
 
 ### Across Platforms/跨平台
 
 [test.py](./test.py) 在 Windows 系统（Windows10）上运行的界面如下：
 
-<p><img height="383px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/test_win32.png" alt="test_win32.png"/></p>
+![test_win32.png](docs/images/test_win32.png)
 
 [test.py](./test.py) 在 Linux 系统（Ubuntu22.04）上运行的界面如下：
 
-<p><img height="408px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/test_linux.png" alt="test_linux.png"/></p>
+![test_linux.png](docs/images/test_linux.png)
 
 Contents/模块内容
 -------------------
 
 Each non internal class and function in the module will be described in detail here  
 这里会详细说明模块中的每个非内部类和函数
 
@@ -160,15 +283,16 @@
 
 ### Virtual Canvas Widget/虚拟画布控件
 
 1. `Label`: 标签控件
 
     标签控件的功能和`tkinter.Label`的功能类似，但更加的多元化  
     下面是`Label`控件的外观：  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/LabelTest.png" alt="LabelTest.png" /></p>
+
+    ![LabelTest.png](docs/images/LabelTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('LabelTest', 1000, 400)
@@ -193,16 +317,17 @@
     ```
 
     </details>
 
 2. `Button`: 按钮控件
 
     按钮控件相较于`tkinter.Button`，其自由度更高，`tkinter.Button`只有在按下的时候才能触发绑定的关联事件，而`Button`却可以在鼠标移至按钮上方时、鼠标按下时、鼠标松开时都可以绑定关联事件  
-    下面是`Button`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ButtonTest.png" alt="ButtonTest.png" /></p>
+    下面是`Button`控件的外观：
+
+    ![ButtonTest.png](docs/images/ButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ButtonTest', 500, 500)
@@ -228,15 +353,16 @@
 
     </details>
 
 3. `CheckButton`: 复选框控件
 
     复选框控件相对于`tkinter`原生的`tkinter.CheckButton`在使用方面更加地简单，同时颜值也上升了不少  
     下面是`CheckButton`控件的外观：
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/CheckButtonTest.png" alt="CheckButtonTest.png"/></p>
+
+    ![CheckButtonTest.png](docs/images/CheckButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('CheckButtonTest', 500, 300)
@@ -262,16 +388,17 @@
     ```
 
     </details>
 
 4. `Entry`: 输入框控件
 
     输入框控件可以轻松地设置输入的文本位置（靠左、居中和靠右），同时，它可以在鼠标移至输入框上方、鼠标未在输入框上方两种状态显示不同的默认文本  
-    下面是`Entry`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/EntryTest.png" alt="EntryTest.png" /></p>
+    下面是`Entry`控件的外观：
+
+    ![EntryTest.png](docs/images/EntryTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('EntryTest', 500, 400)
@@ -307,16 +434,17 @@
     ```
 
     </details>
 
 5. `Text`: 文本框控件
 
     文本框类似于输入框，这里就不再赘述  
-    下面是`Text`控件的外观：  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/TextTest.png" alt="TextTest.png" /></p>
+    下面是`Text`控件的外观：
+
+    ![TextTest.png](docs/images/TextTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('TextTest', 1000, 400)
@@ -342,16 +470,17 @@
     ```
 
     </details>
 
 6. `Progressbar`: 进度条控件
 
     进度条控件相比`tkinter.ttk.Progressbar`，外观上的自由度较大  
-    下面是`Progressbar`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ProgressbarTest.png" alt="ProgressbarTest.png" /></p>
+    下面是`Progressbar`控件的外观：
+
+    ![ProgressbarTest.png](docs/images/ProgressbarTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ProgressbarTest', 500, 500)
@@ -403,16 +532,17 @@
 
     单例模式，不用介绍了吧？通过继承它来使用
 
 ### Tool Function/工具函数
 
 1. `move`: <a name="move">移动函数</a>
 
-    移动函数可以轻松地按一定的规律、移动速度、移动时间去移动`tkintertools`模块内的所有对象，同时兼容了`tkinter`内的对象，即`tkinter`中的对象也可以很方便地移动，甚至它还可以移动窗口的位置！  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/MoveTest.gif" alt="MoveTest.gif" /></p>
+    移动函数可以轻松地按一定的规律、移动速度、移动时间去移动`tkintertools`模块内的所有对象，同时兼容了`tkinter`内的对象，即`tkinter`中的对象也可以很方便地移动，甚至它还可以移动窗口的位置！
+
+    ![MoveTest.gif](docs/images/MoveTest.gif)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('MoveTest', 500, 500)
@@ -456,17 +586,19 @@
     `left`   : "tkintertools        "  
     `center` : "    tkintertools    "  
     `right`  : "        tkintertools"</pre>
 
 3. `color`: <a name="Gradient">颜色函数</a>
 
     颜色函数可以轻松求出一个颜色到另外一个颜色的过渡颜色，因此可以轻松得到渐变色的效果，同时，改变传入的参数还可以得到传入颜色的对比色  
-    第二张图是 test.py 在图像测试中绘制的图案  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ColorTest.png" alt="ColorTest.png" />
-    <img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/Test_Draw.png" alt="Test_Draw.png" /></p>
+    第二张图是 test.py 在图像测试中绘制的图案
+
+    ![ColorTest.png](docs/images/ColorTest.png)
+
+    ![Test_Draw.png](docs/images/Test_Draw.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ColorTest', 500, 500)
@@ -496,19 +628,19 @@
     <p><img width="540px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/font.png" alt="font.png" /></p>
 
 5. `SetProcessDpiAwareness`: <a name="DPI">DPI 级别设置函数</a>
 
     这个函数实际上只是对函数`ctypes.WinDLL('shcore').SetProcessDpiAwareness`的一个简单包装，其值可为 0、1 和 2，分别代表程序 DPI 的不同级别，那么缩放效果也就不同，`tkintertools`选择的值是 1，但程序默认值实际为 0  
     下面是未执行这个函数的效果
     
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/SetProcessDpiAwareness_0.png" alt="SetProcessDpiAwareness_0.png" /></p>
+    ![SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
 
     <p>下面是执行了这个函数的效果</p>
 
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/SetProcessDpiAwareness_1.png" alt="SetProcessDpiAwareness_1.png" /></p>
+    ![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
 
     从上面的两张图中可以很明显的看出第一张很模糊，第二张很清晰，这就是 DPI 级别不同的原因，不过这一点在屏幕缩放比不是 100% 的时候才会出现  
     大家对上面的图肯定很熟悉，这不就是 IDLE 吗！？对，这个的问题的解决办法也是来自于 IDLE 的源代码 [pyshell.py line 18~20]  
     注意：该函数在程序的不同位置执行的效果不一样！一般用在`mainloop`之前，但`tkintertools`已经在`mainloop`函数中嵌入了该函数，无需再设置一次 DPI 级别，此函数是为了原生`tkinter`程序用的。
 
 Examples/实战示例
 ----------------
@@ -551,25 +683,23 @@
 * 文章链接: 暂无
 * 代码仓库: https://gitcode.net/weixin_62651706/tester
 * 程序下载: 暂无
 * 推荐指数: 👍👍👍
 
 这个案例使用了最新稳定版的 tkintertools-v2.6.0，界面非常稳定，几乎没有 bug，完全采用 tkintertools 的控件，颜值很高，界面非常流畅。体现了 tkintertools 模块与 tkinter 模块相比在性能上的优越性！
 
-<p>
-    <img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/examples/exam3_1.png" alt="client.png"/>
-    <img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/examples/exam3_2.png" alt="client.png"/>
-</p>
+![exam3_1.png](docs/examples/exam3_1.png)
+![exam3_2.png](docs/examples/exam3_2.png)
 
 More/更多
 ---------
 
-> GitCode:  
-> https://gitcode.net/weixin_62651706/tkintertools
+> GitHub:  
+> https://github.com/Xiaokang2022/tkintertools
 
-> GitHub(Mirror/镜像):  
-> https://github.com/XiaoKang2022-CSDN/tkintertools
+> GitCode(Mirror/镜像):  
+> https://gitcode.net/weixin_62651706/tkintertools
 
-> Column/专栏:  
-> https://blog.csdn.net/weixin_62651706/category_11600888.html
+> Gitee(Mirror/镜像):  
+> https://gitee.com/xiaokang-2022/tkintertools
 
 还有更多内容请在 [源代码](./tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,26 +1,73 @@
+Metadata-Version: 2.1 Name: tkintertools Version: 2.6.2 Summary: An auxiliary
+module of the tkinder module Home-page: https://gitcode.net/weixin_62651706/
+tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com License:
+MulanPSL-2.0 Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
+Classifier: Operating System :: OS Independent Description-Content-Type: text/
+markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
                             [Email] [Blog] [Author]
 Installation/æ¨¡åå®è£ ----------------------- ### Stable version/
-ç¨³å®çæ¬ * Version/çæ¬ : 2.6.1 * Release Date/åå¸æ¥æ : 2023/05/21
-``` pip install tkintertools==2.6.1 ``` æè ``` pip install tkintertools ```
-è¿ä¸ªæ¯ç®åçææ°çï¼æ¯è¾ç¨³å®ï¼bug
+ç¨³å®çæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/30
+``` pip install tkintertools==2.6.2 ``` æè ``` pip install tkintertools ```
+è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
 æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã ç¨³å®çæææ¡£å¯ä»¥æ¥çï¼æ
 issue æä¼å»æ¥çå¹¶å°è¯è§£å³ issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.1 * Release Date/åå¸æ¥æ : 2023/05/21
-``` pip install tkintertools-dev==2.6.1 ```
+å¼åçæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/26
+``` pip install tkintertools-dev==2.6.2 ```
 è¿ä¸ªæ¯ä½èæ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
 å¯è½ä¼æ¯è¾å¤ã å¼åçæ¬æ²¡æå¯¹åºçææ¡£ï¼å¤§å®¶å¯ä»¥å¨ issue
 ä¸­æåºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
-Description/æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº
-tkinter
+News/ææ°åè½ -----------
+-
+ææ°çç`tkintertools`ä¸º`2.6.2`ï¼æ°å¢ä¸é¡¹æä¸ºå¼ºå¤§çåè½ï¼3dç»å¾ï¼
+åæ¶ä¿®å¤ä¸äºbugï¼ä¼åäºä¸é¨åä»£ç ï¼æåäºä¸é¨åæ§è½ã
+éè¿ä»¥ä¸ä»£ç æ¥ä½¿ç¨3dç»å¾åè½ï¼ ```python from tkintertools import
+tools_3d as t3d import tkintertools.tools_3d as t3d #
+ä¸¤ç§å¼å¥æ¹å¼é½å¯ä»¥ ``` å­æ¨¡å: [tools_3d.py](./tkintertools/
+tools_3d.py)
+ç®å3dç»å¾åè½è¿æ¯è¾ç®éï¼ä»è½ç»å¶ç¹ãçº¿ãé¢ä»¥åç´è¾¹çç©ºé´å ä½ä½ï¼å¯¹äºæ²è¾¹çç©ºé´å ä½ä½è¿å¨å¼åä¸­ï¼
+ä»¥ä¸æ¯ä¸ä¸ªä½¿ç¨3dç»å¾çç¤ºä¾ï¼
+å¨è¿ä¸ªç¤ºä¾ä¸­ï¼æä½é¼ æ å·¦é®å¯ä»¥æè½¬å ä½ä½ï¼æä½é¼ æ å³é®å¯ä»¥å¹³ç§»å ä½ä½ï¼æ»å¨é¼ æ æ»è½®å¯ä»¥ç¼©æ¾å ä½ä½ï¼
+xãy å z è½´åå«æ¯çº¢è²ãç»¿è²åèè²ççº¿ã ![3dç»å¾](./docs/
+images/3d.png) æºä»£ç  ```python import random import tkinter import
+tkintertools as tkt from tkintertools import tools_3d as t3d root = tkt.Tk
+('tools_3d', 1280, 720) canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0) geos = []
+# type: list[t3d.Geometry] origin = t3d.Point(canvas, [0, 0, 0], size=5) #
+åç¹ axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'), #
+åå»ºåæ è½´ t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3,
+fill='green'), t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
+for _ in range(8): # åå»ºæ­£æ¹ä½ cube = t3d.Cuboid( canvas, *random.sample
+(range(-200, 200), 3), *random.sample(range(50, 100), 3)) geos.append(cube) #
+åå»ºåé¢ä½ x, y, z = random.sample(range(-200, 200), 3) tetr =
+t3d.Tetrahedron( canvas, *[[x+random.randint(-100, 100), y+random.randint(-100,
+100), z+random.randint(-100, 100)] for _ in range(4)]) geos.append(tetr) def
+translate(event, flag=False, _cache=[]): # type: (tkinter.Event, bool, list
+[float]) -> None """ å¹³ç§»äºä»¶ """ if flag: _cache[:] = [event.x, event.y]
+return dx = (event.x - _cache[0]) / 6 dy = (event.y - _cache[1]) / 6 _cache[:
+] = [event.x, event.y] for axis in axes: axis.translate(0, 6*dx, 6*dy)
+axis.update() for geo in geos: geo.translate(0, dx, dy) geo.update()
+origin.translate(0, 6*dx, 6*dy) origin.update() def rotate(event, flag=False,
+_cache=[]): # type: (tkinter.Event, bool, list[float]) -> None """ æè½¬äºä»¶
+""" if flag: _cache[:] = [event.x, event.y] return dy = (event.x - _cache[0]) /
+200 dx = (_cache[1] - event.y) / 200 _cache[:] = [event.x, event.y] for axis in
+axes: axis.rotate(0, 6*dx, 6*dy, center=origin.coords) axis.update() for geo in
+geos: geo.rotate(0, dx, dy, center=origin.coords) geo.update() def scale
+(event): # type: (tkinter.Event) -> None """ ç¼©æ¾äºä»¶ """ k = 1.01 if
+event.delta > 0 else 0.99 for geo in geos: geo.scale(k, k, k) geo.update()
+root.bind('', lambda event: rotate(event, True)) root.bind('', rotate)
+root.bind('', lambda event: translate(event, True)) root.bind('', translate)
+root.bind('', scale) root.mainloop() ```  æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼
+[CHANGELOG.md](./CHANGELOG.md) Description/æ¨¡åè¯´æ ---------------------
+- tkintertools æ¯ä¸æ¬¾åºäº tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
 tkinter æ¨¡åä¸­ Canvas å¯¹è±¡ä¸­ç»å¶èæçï¼è¿å°±èµäºäº
 tkintertools æ§ä»¶ä¸äºå¨ tkinter ä¸­æ²¡æçç¹æ§ï¼åä¸¾å¦ä¸ï¼ *
 æ§ä»¶èæ¯å¯ä»¥æ¯éæçï¼å®éä¸æ¯æ²¡æèæ¯é¢è²ï¼ *
 æ§ä»¶çæ ·å¼å¯ä»¥æ¯èªå®ä¹çï¼æ¯å¦æé®æåè§ï¼ *
 æ§ä»¶çåå»ºéåº¦è¿å¤§äº tkinter çæ§ä»¶ï¼é¤äº Canvas æ§ä»¶ï¼
@@ -51,78 +98,71 @@
 (#Gradient) ### Automatically adapt to DPI/èªå¨éåºDPI è§ [DPI
 çº§å«è®¾ç½®å½æ°](#DPI) ### Detailed type hints/è¯¦ç»çç±»åæç¤º åè
 [PEP 526](https://peps.python.org/pep-0526/)ã[PEP 586](https://
 peps.python.org/pep-0586/)ã[PEP 604](https://peps.python.org/pep-0604/) å
 [PEP 612](https://peps.python.org/pep-0612/
 )ï¼æéç¨äºæå¼å®¹çæ¹å¼å»å®ç°è¯¦ç»çç±»åæç¤ºï¼å¯éç¨
 IDE æ VScodeãPycharm ç­ã
-é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼
-[type_hint.png]
-å¨ VSCode
+é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼ !
+[type_hint.png](docs/images/type_hint_vscode.png) å¨ VSCode
 ç¼è¾å¨ä¸­ï¼å½é¼ æ ç§»è³ç±»æèå½æ°çåå­ä¸é¢æ¶ï¼ä¼èªå¨æ¾ç¤ºè¯¥ç±»æèå½æ°çæ³¨éææ¡£ãéè¿è¿ç§æ¹å¼ï¼ä¸éè¦çå¤ªå¤çå¸®å©ææ¡£åèµæå°±è½çç»å°ä½¿ç¨
 tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](./test.py) å¨
-Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼
-[test_win32.png]
-[test.py](./test.py) å¨ Linux
-ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼
-[test_linux.png]
-Contents/æ¨¡ååå®¹ ------------------- Each non internal class and function
-in the module will be described in detail here
+Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_win32.png]
+(docs/images/test_win32.png) [test.py](./test.py) å¨ Linux
+ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png](docs/
+images/test_linux.png) Contents/æ¨¡ååå®¹ ------------------- Each non
+internal class and function in the module will be described in detail here
 è¿éä¼è¯¦ç»è¯´ææ¨¡åä¸­çæ¯ä¸ªéåé¨ç±»åå½æ° ### Container
 Widget/å®¹å¨æ§ä»¶ 1. `Tk`: çªå£ç±»
 ç»§æ¿äº`tkinter.Tk`ï¼å¨ç»§æ¿äº`tkinter`æ¨¡åå`Tk`çåºç¡ä¸ï¼åå å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¹¶å å¥äºæ£æµçªå£å¤§å°æ¯å¦ç¼©æ¾çæºå¶ï¼ä»¥ä½¿å¾å¶å­`Canvas`åè½æ­£ç¡®å°è¿è¡ç¼©æ¾
 2. `Toplevel`: é¡¶çº§çªå£ç±»
 ç»§æ¿äº`tkinter.Toplevel`å`Tk`ï¼å å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¶ä½åä¸`Tk`ä¸æ ·
 3. `Canvas`: ç»å¸ç±»
 ç»§æ¿äº`tkinter.Canvas`ï¼å å¥äºå¯¹ç»å¸èææ§ä»¶çæ¯æï¼åæ¶æ¯åç±»ååºäºä»¶ãç¼©æ¾æ§å¶çç®¡çèï¼ä¹å¯¹`tkinter.Canvas`çå®ä¾æ¹æ³æä¸å®çå¼å®¹æ§
 ### Virtual Canvas Widget/èæç»å¸æ§ä»¶ 1. `Label`: æ ç­¾æ§ä»¶
 æ ç­¾æ§ä»¶çåè½å`tkinter.Label`çåè½ç±»ä¼¼ï¼ä½æ´å çå¤åå
-ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼
-[LabelTest.png]
+ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼ ![LabelTest.png](docs/images/LabelTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('LabelTest', 1000,
 400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Label(canvas, 50, 50, 400, 100, text='NormalLabel\nHere is the text')
 tkt.Label(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerLabel')
 tkt.Label(canvas, 550, 50, 400, 100, text='DisableLabel').set_live(False)
 tkt.Label(canvas, 550, 200, 400, 100, radius=20, text='TransparentLabel',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  2. `Button`: æé®æ§ä»¶
 æé®æ§ä»¶ç¸è¾äº`tkinter.Button`ï¼å¶èªç±åº¦æ´é«ï¼`tkinter.Button`åªæå¨æä¸çæ¶åæè½è§¦åç»å®çå³èäºä»¶ï¼è`Button`å´å¯ä»¥å¨é¼ æ ç§»è³æé®ä¸æ¹æ¶ãé¼ æ æä¸æ¶ãé¼ æ æ¾å¼æ¶é½å¯ä»¥ç»å®å³èäºä»¶
-ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼
-[ButtonTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ButtonTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
-height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
-range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼ ![ButtonTest.png](docs/images/
+ButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk
+('ButtonTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful
+(x, y, width, height): # type: (int, int, int, int) -> None """ Gradient colors
+""" for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 280, 400,
 100) tkt.Button(canvas, 150, 135, 200, 50, text='NormalButton') tkt.Button
 (canvas, 100, 195, 300, 50, radius=10, text='RoundCornerButton') tkt.Button
 (canvas, 150, 255, 200, 50, text='DisableButton').set_live(False) tkt.Button
 (canvas, 100, 315, 300, 50, radius=10, text='TransparentButton',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  3. `CheckButton`:
 å¤éæ¡æ§ä»¶
 å¤éæ¡æ§ä»¶ç¸å¯¹äº`tkinter`åçç`tkinter.CheckButton`å¨ä½¿ç¨æ¹é¢æ´å å°ç®åï¼åæ¶é¢å¼ä¹ä¸åäºä¸å°
-ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼
-[CheckButtonTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('CheckButtonTest',
-500, 300) canvas = tkt.Canvas(root, 500, 300, 0, 0) def colorful(x, y, width,
-height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
-range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
-canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(40, 190, 420,
-50) tkt.CheckButton(canvas, 50, 50, 30, text='NormalCheckButton', value=True)
-tkt.CheckButton(canvas, 50, 100, 30, text='DisableCheckButton',
-value=True).set_live(False) tkt.CheckButton(canvas, 50, 150, 30, radius=10,
-text='RoundCornerCheckButton') tkt.CheckButton(canvas, 50, 200, 30, radius=15,
-text='TransparentCheckButton', color_fill=tkt.COLOR_NONE) root.mainloop() ```
-4. `Entry`: è¾å¥æ¡æ§ä»¶
+ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼ ![CheckButtonTest.png](docs/images/
+CheckButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root =
+tkt.Tk('CheckButtonTest', 500, 300) canvas = tkt.Canvas(root, 500, 300, 0, 0)
+def colorful(x, y, width, height): # type: (int, int, int, int) -> None """
+Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
+'#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
+colorful(40, 190, 420, 50) tkt.CheckButton(canvas, 50, 50, 30,
+text='NormalCheckButton', value=True) tkt.CheckButton(canvas, 50, 100, 30,
+text='DisableCheckButton', value=True).set_live(False) tkt.CheckButton(canvas,
+50, 150, 30, radius=10, text='RoundCornerCheckButton') tkt.CheckButton(canvas,
+50, 200, 30, radius=15, text='TransparentCheckButton',
+color_fill=tkt.COLOR_NONE) root.mainloop() ```  4. `Entry`: è¾å¥æ¡æ§ä»¶
 è¾å¥æ¡æ§ä»¶å¯ä»¥è½»æ¾å°è®¾ç½®è¾å¥çææ¬ä½ç½®ï¼é å·¦ãå±ä¸­åé å³ï¼ï¼åæ¶ï¼å®å¯ä»¥å¨é¼ æ ç§»è³è¾å¥æ¡ä¸æ¹ãé¼ æ æªå¨è¾å¥æ¡ä¸æ¹ä¸¤ç§ç¶ææ¾ç¤ºä¸åçé»è®¤ææ¬
-ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼
-[EntryTest.png]
+ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼ ![EntryTest.png](docs/images/EntryTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('EntryTest', 500,
 400) canvas = tkt.Canvas(root, 500, 400, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 193, 400,
 100) tkt.Entry(canvas, 20, 20, 200, 30, text=('LeftEntry', 'Enter')) tkt.Entry
 (canvas, 20, 55, 200, 30, text=( 'CenterEntry', 'Enter'), justify='center')
@@ -133,79 +173,77 @@
 radius=8, text='RightEntry', justify='right') tkt.Entry(canvas, 100, 150, 300,
 35, text=('PasswordEntry', 'Click To Enter'), justify='center', show='â')
 tkt.Entry(canvas, 100, 200, 300, 35, text='DisableEntry',
 justify='center').set_live(False) tkt.Entry(canvas, 100, 250, 300, 35,
 text='TransparentEntry', justify='center', color_fill=tkt.COLOR_NONE)
 root.mainloop() ```  5. `Text`: ææ¬æ¡æ§ä»¶
 ææ¬æ¡ç±»ä¼¼äºè¾å¥æ¡ï¼è¿éå°±ä¸åèµè¿°
-ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼
-[TextTest.png]
+ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼ ![TextTest.png](docs/images/TextTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('TextTest', 1000,
 400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
 height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
 for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Text(canvas, 50, 50, 400, 100, text=('NormalText(Left)', 'Click To
 Enter')) tkt.Text(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerText
 (Center)', justify='center') tkt.Text(canvas, 550, 50, 400, 100,
 text='DisableText').set_live(False) tkt.Text(canvas, 550, 200, 400, 100,
 radius=20, text='TransparentText(Right)', justify='right',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  6. `Progressbar`:
 è¿åº¦æ¡æ§ä»¶
 è¿åº¦æ¡æ§ä»¶ç¸æ¯`tkinter.ttk.Progressbar`ï¼å¤è§ä¸çèªç±åº¦è¾å¤§
-ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼
-[ProgressbarTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ProgressbarTest',
-500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
-height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
-for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
-canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(30, 290, 440,
-50) tkt.Progressbar(canvas, 50, 50, 400, 30) tkt.Progressbar(canvas, 50, 100,
-400, 30).load(.6667) tkt.Progressbar(canvas, 50, 150, 400, 30,
-borderwidth=5).load(1) (_ := tkt.Progressbar(canvas, 50, 200, 400, 30)).load
-(0.3333) _.set_live(False) tkt.Progressbar(canvas, 50, 250, 400, 30, color_bar=
-( 'lightyellow', 'skyblue')).load(.5) tkt.Progressbar(canvas, 50, 300, 400, 30,
-color_bar=('', 'orange')).load(.1667) progressbar = tkt.Progressbar(canvas, 50,
-375, 400, 30) progressbar_2 = tkt.Progressbar(canvas, 50, 425, 400, 30) def
-load(total, count=0): # type: (int, int) -> None """ load progressbar """
-progressbar.load(count/total) progressbar_2.load(1-count/total) if count <
-total: root.after(3, load, total, count+1) load(10000) root.mainloop() ```  ###
-Tool Class/å·¥å·ç±» 1. `PhotoImage`: å¾çç±»
+ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼ ![ProgressbarTest.png](docs/images/
+ProgressbarTest.png) æºä»£ç  ```python import tkintertools as tkt root =
+tkt.Tk('ProgressbarTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0)
+def colorful(x, y, width, height) -> None: # type: (int, int, int, int) -> None
+""" Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
+'#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
+colorful(30, 290, 440, 50) tkt.Progressbar(canvas, 50, 50, 400, 30)
+tkt.Progressbar(canvas, 50, 100, 400, 30).load(.6667) tkt.Progressbar(canvas,
+50, 150, 400, 30, borderwidth=5).load(1) (_ := tkt.Progressbar(canvas, 50, 200,
+400, 30)).load(0.3333) _.set_live(False) tkt.Progressbar(canvas, 50, 250, 400,
+30, color_bar=( 'lightyellow', 'skyblue')).load(.5) tkt.Progressbar(canvas, 50,
+300, 400, 30, color_bar=('', 'orange')).load(.1667) progressbar =
+tkt.Progressbar(canvas, 50, 375, 400, 30) progressbar_2 = tkt.Progressbar
+(canvas, 50, 425, 400, 30) def load(total, count=0): # type: (int, int) -> None
+""" load progressbar """ progressbar.load(count/total) progressbar_2.load(1-
+count/total) if count < total: root.after(3, load, total, count+1) load(10000)
+root.mainloop() ```  ### Tool Class/å·¥å·ç±» 1. `PhotoImage`: å¾çç±»
 `PhotoImage`ç±»ç»§æ¿äº`tkinter.PhotoImage`ï¼å®æ¯å¨`tkinter.PhotoImage`çåºç¡ä¸ååè½çå¼ºåï¼å¯¹
 gif
 å¨å¾æå¾å¥½çæ¯æï¼ä»éæå°éä»£ç å³å¯å®ç°å¨å¾çæ¾ç¤ºï¼è¿å¯ä»¥è®¾ç½®å¨å¾æ¾ç¤ºçéåº¦ï¼æ­¤å¤ï¼å¯¹
 png
 ç±»åçå¾ççæ¯æä¹æå¼ºåï¼å¯ä»¥å¨ä¸ä¾èµä»»ä½ç¬¬ä¸æ¹æ¨¡åæèåºçæåµä¸ï¼å¯¹
 png å¾çè¿è¡ç¼©æ¾ 2. `Singleton`: åä¾æ¨¡å¼ç±»
 åä¾æ¨¡å¼ï¼ä¸ç¨ä»ç»äºå§ï¼éè¿ç»§æ¿å®æ¥ä½¿ç¨ ### Tool Function/
 å·¥å·å½æ° 1. `move`: ç§»å¨å½æ°
 ç§»å¨å½æ°å¯ä»¥è½»æ¾å°æä¸å®çè§å¾ãç§»å¨éåº¦ãç§»å¨æ¶é´å»ç§»å¨`tkintertools`æ¨¡ååçææå¯¹è±¡ï¼åæ¶å¼å®¹äº`tkinter`åçå¯¹è±¡ï¼å³`tkinter`ä¸­çå¯¹è±¡ä¹å¯ä»¥å¾æ¹ä¾¿å°ç§»å¨ï¼çè³å®è¿å¯ä»¥ç§»å¨çªå£çä½ç½®ï¼
-[MoveTest.gif]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('MoveTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500, 0, 0) rect = canvas.create_rectangle
-(50, 350, 150, 450) def move_window(switch=[True]): # type: (list[bool]) -
-> None tkt.move(root, None, 1000 if switch[0] else -1000, 0, 800, mode='flat')
-switch[0] = not switch[0] def move_button(switch=[True]) -> None: # type: (list
-[bool]) -> None tkt.move(canvas, button, 200 if switch[0] else -200, 0, 500,
-mode='rebound') switch[0] = not switch[0] def move_rect(switch=[True]): # type:
-(list[bool]) -> None tkt.move(canvas, rect, 200 if switch[0] else -200, 0, 500,
-mode='smooth') switch[0] = not switch[0] tkt.Button(canvas, 50, 50, 200, 40,
-radius=10, text='MoveWindow', command=move_window) tkt.Button(canvas, 50, 100,
-200, 40, radius=10, text='MoveRect', command=move_rect) button = tkt.Button
-(canvas, 50, 150, 200, 40, radius=10, text='MoveButton', command=move_button)
-root.mainloop() ```  2. `text`: ææ¬å½æ°
+![MoveTest.gif](docs/images/MoveTest.gif) æºä»£ç  ```python import
+tkintertools as tkt root = tkt.Tk('MoveTest', 500, 500) canvas = tkt.Canvas
+(root, 500, 500, 0, 0) rect = canvas.create_rectangle(50, 350, 150, 450) def
+move_window(switch=[True]): # type: (list[bool]) -> None tkt.move(root, None,
+1000 if switch[0] else -1000, 0, 800, mode='flat') switch[0] = not switch[0]
+def move_button(switch=[True]) -> None: # type: (list[bool]) -> None tkt.move
+(canvas, button, 200 if switch[0] else -200, 0, 500, mode='rebound') switch[0]
+= not switch[0] def move_rect(switch=[True]): # type: (list[bool]) -> None
+tkt.move(canvas, rect, 200 if switch[0] else -200, 0, 500, mode='smooth')
+switch[0] = not switch[0] tkt.Button(canvas, 50, 50, 200, 40, radius=10,
+text='MoveWindow', command=move_window) tkt.Button(canvas, 50, 100, 200, 40,
+radius=10, text='MoveRect', command=move_rect) button = tkt.Button(canvas, 50,
+150, 200, 40, radius=10, text='MoveButton', command=move_button) root.mainloop
+() ```  2. `text`: ææ¬å½æ°
 å¯ä»¥å¿«éå¹¶æ¹ä¾¿å°å¾å°ä¸ä¸ªåæ°é¿åº¦çå­ç¬¦ä¸²ï¼ä¸å­ç¬¦ä¸²çåå®¹å¯ä»¥æå®ä½ç½®
 å¦ï¼å¾å°ä¸ä¸ª 20 é¿åº¦çå­ç¬¦ä¸² âtkintertoolsâ
     `left`   : "tkintertools        "
     `center` : "    tkintertools    "
     `right`  : "        tkintertools"
 3. `color`: é¢è²å½æ°
 é¢è²å½æ°å¯ä»¥è½»æ¾æ±åºä¸ä¸ªé¢è²å°å¦å¤ä¸ä¸ªé¢è²çè¿æ¸¡é¢è²ï¼å æ­¤å¯ä»¥è½»æ¾å¾å°æ¸åè²çææï¼åæ¶ï¼æ¹åä¼ å¥çåæ°è¿å¯ä»¥å¾å°ä¼ å¥é¢è²çå¯¹æ¯è²
-ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡
-[ColorTest.png] [Test_Draw.png]
+ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡ ![ColorTest.png]
+(docs/images/ColorTest.png) ![Test_Draw.png](docs/images/Test_Draw.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ColorTest', 500,
 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 =
 tkt.color(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i,
 y+height, fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
 outline=color_2, width=2) colorful(50, 50, 400, 100) root.mainloop() ```  4.
@@ -215,18 +253,18 @@
 tcl çå½ä»¤ï¼ä½¿å¾å­ä½éæ©æ¡è½å¤è¢«æä»¬ä½¿ç¨ã
 [font.png]
 5. `SetProcessDpiAwareness`: DPI çº§å«è®¾ç½®å½æ°
 è¿ä¸ªå½æ°å®éä¸åªæ¯å¯¹å½æ°`ctypes.WinDLL
 ('shcore').SetProcessDpiAwareness`çä¸ä¸ªç®ååè£ï¼å¶å¼å¯ä¸º 0ã1
 å 2ï¼åå«ä»£è¡¨ç¨åº DPI
 çä¸åçº§å«ï¼é£ä¹ç¼©æ¾ææä¹å°±ä¸åï¼`tkintertools`éæ©çå¼æ¯
-1ï¼ä½ç¨åºé»è®¤å¼å®éä¸º 0 ä¸é¢æ¯æªæ§è¡è¿ä¸ªå½æ°çææ
-[SetProcessDpiAwareness_0.png]
+1ï¼ä½ç¨åºé»è®¤å¼å®éä¸º 0 ä¸é¢æ¯æªæ§è¡è¿ä¸ªå½æ°çææ !
+[SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
 ä¸é¢æ¯æ§è¡äºè¿ä¸ªå½æ°çææ
-[SetProcessDpiAwareness_1.png]
+![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
 ä»ä¸é¢çä¸¤å¼ å¾ä¸­å¯ä»¥å¾ææ¾ççåºç¬¬ä¸å¼ å¾æ¨¡ç³ï¼ç¬¬äºå¼ å¾æ¸æ°ï¼è¿å°±æ¯
 DPI çº§å«ä¸åçåå ï¼ä¸è¿è¿ä¸ç¹å¨å±å¹ç¼©æ¾æ¯ä¸æ¯ 100%
 çæ¶åæä¼åºç° å¤§å®¶å¯¹ä¸é¢çå¾è¯å®å¾çæï¼è¿ä¸å°±æ¯ IDLE
 åï¼ï¼å¯¹ï¼è¿ä¸ªçé®é¢çè§£å³åæ³ä¹æ¯æ¥èªäº IDLE çæºä»£ç 
 [pyshell.py line 18~20]
 æ³¨æï¼è¯¥å½æ°å¨ç¨åºçä¸åä½ç½®æ§è¡çææä¸ä¸æ ·ï¼ä¸è¬ç¨å¨`mainloop`ä¹åï¼ä½`tkintertools`å·²ç»å¨`mainloop`å½æ°ä¸­åµå¥äºè¯¥å½æ°ï¼æ éåè®¾ç½®ä¸æ¬¡
 DPI çº§å«ï¼æ­¤å½æ°æ¯ä¸ºäºåç`tkinter`ç¨åºç¨çã Examples/
@@ -255,14 +293,13 @@
 æ¨¡åçå¼å®¹æ§ï¼
 [chess.png] [chess.png]
 ### ç®æç»å½çé¢ * æç« é¾æ¥: ææ  * ä»£ç ä»åº: https://
 gitcode.net/weixin_62651706/tester * ç¨åºä¸è½½: ææ  * æ¨èææ°:
 ððð è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
-æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼
-[client.png] [client.png]
-More/æ´å¤ --------- > GitCode: > https://gitcode.net/weixin_62651706/
-tkintertools > GitHub(Mirror/éå): > https://github.com/XiaoKang2022-CSDN/
-tkintertools > Column/ä¸æ : > https://blog.csdn.net/weixin_62651706/
-category_11600888.html è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/
-) ä¸­æ¢ç´¢ï¼
+æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png](docs/
+examples/exam3_1.png) ![exam3_2.png](docs/examples/exam3_2.png) More/æ´å¤ ---
+------ > GitHub: > https://github.com/Xiaokang2022/tkintertools > GitCode
+(Mirror/éå): > https://gitcode.net/weixin_62651706/tkintertools > Gitee
+(Mirror/éå): > https://gitee.com/xiaokang-2022/tkintertools
+è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
```

### Comparing `tkintertools-2.6.1.2/setup.py` & `tkintertools-2.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ 上传 pypi """
 
 import setuptools
 
 
 setuptools.setup(
     name='tkintertools',
-    version="2.6.1.2",
+    version="2.6.2",
     author='Xiaokang2022',
     license='MulanPSL-2.0',
     author_email='2951256653@qq.com',
     description='An auxiliary module of the tkinder module',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://gitcode.net/weixin_62651706/tkintertools',
```

### Comparing `tkintertools-2.6.1.2/tkintertools/__init__.py` & `tkintertools-2.6.2/tkintertools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,21 +33,20 @@
 if sys.version_info < (3, 7):  # Version Check
     error_info = '\n\033[31mOperation Requirements: \033[32m\nPython version shall not be less than\033[33m 3.7.0 !\033[0m'
     raise RuntimeError(error_info)
 
 from .__main__ import (Button, Canvas, CheckButton, Entry, Label, PhotoImage,
                        Progressbar, SetProcessDpiAwareness, Singleton, Text,
                        Tk, Toplevel, askfont, color, move, text)
-from .constants import *
 
 __author__ = 'Xiaokang2022<2951256653@qq.com>'
-__version__ = '2.6.1'
+__version__ = '2.6.2'
 __all__ = [
     # Container Widgets
     'Tk', 'Toplevel', 'Canvas',
     # Virtual Canvas Widgets
     'Label', 'Button', 'CheckButton', 'Entry', 'Text', 'Progressbar',
     # Tool Classes
     'PhotoImage', 'Singleton',
     # Tool Functions
-    'move', 'text', 'color', 'askfont', 'SetProcessDpiAwareness'
+    'move', 'text', 'color', 'askfont', 'SetProcessDpiAwareness',
 ]
```

### Comparing `tkintertools-2.6.1.2/tkintertools/__main__.py` & `tkintertools-2.6.2/tkintertools/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Main File """
 
-import math  # 数学函数
+import math  # 数学支持
 import sys  # DPI 兼容
 import tkinter  # 基础模块
 from fractions import Fraction  # 图片缩放
 from typing import Any, Callable, Generator, Iterable  # 类型提示
 
 try:  # NOTE: 为了兼容 Python3.7，从 typing_extensions 引入 Literal 而不是 typing
     from typing_extensions import Literal
```

### Comparing `tkintertools-2.6.1.2/tkintertools/constants.py` & `tkintertools-2.6.2/tkintertools/constants.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 """ All constants """
 
 import sys
 
 PROCESS_SYSTEM_DPI_AWARE = 1
-""" default DPI aware """
+""" Default DPI aware """
 
 
 COLOR_BUTTON_FILL = '#E1E1E1', '#E5F1FB', '#CCE4F7', '#E0E0E0'
-""" default button fill color """
+""" Default button fill color """
 
 COLOR_BUTTON_OUTLINE = '#C0C0C0', '#288CDB', '#4884B4', '#D0D0D0'
-""" default button outline color """
+""" Default button outline color """
 
 COLOR_TEXT_FILL = '#FFFFFF', '#FFFFFF', '#FFFFFF', '#E0E0E0'
-""" default text widget fill color """
+""" Default text widget fill color """
 
 COLOR_TEXT_OUTLINE = '#C0C0C0', '#414141', '#288CDB', '#D0D0D0'
-""" default text widget outline color """
+""" Default text widget outline color """
 
 COLOR_TEXT = '#000000', '#000000', '#000000', '#A3A3A3'
-""" default text color """
+""" Default text color """
 
 COLOR_NONE = '', '', '', ''
-""" default transparent color tuple """
+""" Default transparent color tuple """
 
 COLOR_BAR = '#E1E1E1', '#06b025'
-""" default progress bar color """
+""" Default progress bar color """
 
 BACKGROUND = '#F1F1F1'
-""" default Canvas background color """
+""" Default Canvas background color """
 
 
 BORDERWIDTH = 1
-""" default widget borderwidth """
+""" Default widget borderwidth """
 
 CURSOR = '│'
 """ text cursor """
 
 FONT = 'Microsoft YaHei' if sys.platform == 'win32' else 'DejaVu Sans' if sys.platform == 'linux' else 'Arial'
-""" default font """
+""" Default font """
 
 SIZE = 20
-""" default font size """
+""" Default font size """
 
 LIMIT = -1
-""" default widget text length limit """
+""" Default widget text length limit """
 
 RADIUS = 0
-""" default widget fillet radius """
+""" Default widget fillet radius """
 
 FRAMES = 60
-""" default move frame rate """
+""" Default move frame rate """
 
 TICK = '✓'
-""" default checkbox symbol """
+""" Default checkbox symbol """
+
+
+CFG_3D = 500, None, None
+""" Default 3D configuration """
```

### Comparing `tkintertools-2.6.1.2/tkintertools.egg-info/PKG-INFO` & `tkintertools-2.6.2/tkintertools.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.1.2
+Version: 2.6.2
 Summary: An auxiliary module of the tkinder module
 Home-page: https://gitcode.net/weixin_62651706/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 License: MulanPSL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
@@ -17,24 +17,24 @@
     <p><img height="120px" alt="logo.png"
         src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/tkintertools.png" />
     </p>
     <p>The <code>tkintertools</code> module is an auxiliary module of the <code>tkinter</code> module</p>
     <p><code>tkintertools</code> 模块是 <code>tkinter</code> 模块的辅助模块</p>
     <p>
         <a href="./tkintertools/__init__.py">
-            <img src="https://img.shields.io/badge/Version-2.6.1-blue" alt="latest version" />
+            <img src="https://img.shields.io/badge/Version-2.6.2-blue" alt="latest version" />
         </a>
         <a href="./LICENSE">
             <img src="https://img.shields.io/badge/License-Mulan PSL v2-green" alt="License" />
         </a>
         <a href="./CHANGELOG.md">
-            <img src="https://img.shields.io/badge/ChangeLog-2023/05/21-orange" alt="ChangeLog" />
+            <img src="https://img.shields.io/badge/ChangeLog-2023/05/30-orange" alt="ChangeLog" />
         </a>
         <a href="./TODO.md">
-            <img src="https://img.shields.io/badge/ToDos-10-yellow" alt="ToDos" />
+            <img src="https://img.shields.io/badge/ToDos-13-yellow" alt="ToDos" />
         </a>
         <a href="https://pypistats.org/packages/tkintertools">
             <img src="https://img.shields.io/badge/Downloads-3k-purple" alt="Downloads" />
         </a>
     </p>
     <p>
         <a href="mailto:2951256653@qq.com">
@@ -50,40 +50,149 @@
 </div>
 
 Installation/模块安装
 -----------------------
 
 ### Stable version/稳定版本
 
-* Version/版本 : 2.6.1
-* Release Date/发布日期 : 2023/05/21
+* Version/版本 : 2.6.2
+* Release Date/发布日期 : 2023/05/30
 
 ```
-pip install tkintertools==2.6.1
+pip install tkintertools==2.6.2
 ```
 或者
 ```
 pip install tkintertools
 ```
 
-这个是目前的最新版，比较稳定，bug 没有那么多，推荐使用这个。  
+这个是目前的最新稳定版，比较稳定，bug 没有那么多，推荐使用这个。  
 稳定版有文档可以查看，有 issue 我会去查看并尝试解决 issue。
 
 ### Development version/开发版本
 
-* Version/版本 : 2.6.1
-* Release Date/发布日期 : 2023/05/21
+* Version/版本 : 2.6.2
+* Release Date/发布日期 : 2023/05/26
 
 ```
-pip install tkintertools-dev==2.6.1
+pip install tkintertools-dev==2.6.2
 ```
 
 这个是作者正在开发的版本，有新功能，但不能保证稳定，bug 可能会比较多。  
 开发版本没有对应的文档，大家可以在 issue 中提出建议，我会适当采纳一些并在开发版本中更改或实现。
 
+News/最新功能
+------------
+
+最新版的`tkintertools`为`2.6.2`，新增一项极为强大的功能：3d绘图！  
+同时修复一些bug，优化了一部分代码，提升了一部分性能。
+
+通过以下代码来使用3d绘图功能：
+
+```python
+from tkintertools import tools_3d as t3d
+import tkintertools.tools_3d as t3d
+# 两种引入方式都可以
+```
+
+子模块: [tools_3d.py](./tkintertools/tools_3d.py)
+
+目前3d绘图功能还比较简陋，仅能绘制点、线、面以及直边的空间几何体，对于曲边的空间几何体还在开发中！  
+以下是一个使用3d绘图的示例：
+
+在这个示例中，按住鼠标左键可以旋转几何体，按住鼠标右键可以平移几何体，滚动鼠标滚轮可以缩放几何体！  
+x、y 和 z 轴分别是红色、绿色和蓝色的线。
+
+![3d绘图](./docs/images/3d.png)
+
+<details><summary><b>源代码</b></summary>
+
+```python
+import random
+import tkinter
+
+import tkintertools as tkt
+from tkintertools import tools_3d as t3d
+
+root = tkt.Tk('tools_3d', 1280, 720)
+canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0)
+
+geos = []  # type: list[t3d.Geometry]
+origin = t3d.Point(canvas, [0, 0, 0], size=5)  # 原点
+axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'),  # 创建坐标轴
+        t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3, fill='green'),
+        t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
+
+for _ in range(8):
+    # 创建正方体
+    cube = t3d.Cuboid(
+        canvas, *random.sample(range(-200, 200), 3), *random.sample(range(50, 100), 3))
+    geos.append(cube)
+    # 创建四面体
+    x, y, z = random.sample(range(-200, 200), 3)
+    tetr = t3d.Tetrahedron(
+        canvas, *[[x+random.randint(-100, 100), y+random.randint(-100, 100), z+random.randint(-100, 100)] for _ in range(4)])
+    geos.append(tetr)
+
+
+def translate(event, flag=False, _cache=[]):
+    # type: (tkinter.Event, bool, list[float]) -> None
+    """ 平移事件 """
+    if flag:
+        _cache[:] = [event.x, event.y]
+        return
+    dx = (event.x - _cache[0]) / 6
+    dy = (event.y - _cache[1]) / 6
+    _cache[:] = [event.x, event.y]
+    for axis in axes:
+        axis.translate(0, 6*dx, 6*dy)
+        axis.update()
+    for geo in geos:
+        geo.translate(0, dx, dy)
+        geo.update()
+    origin.translate(0, 6*dx, 6*dy)
+    origin.update()
+
+
+def rotate(event, flag=False, _cache=[]):  # type: (tkinter.Event, bool, list[float]) -> None
+    """ 旋转事件 """
+    if flag:
+        _cache[:] = [event.x, event.y]
+        return
+    dy = (event.x - _cache[0]) / 200
+    dx = (_cache[1] - event.y) / 200
+    _cache[:] = [event.x, event.y]
+    for axis in axes:
+        axis.rotate(0, 6*dx, 6*dy, center=origin.coords)
+        axis.update()
+    for geo in geos:
+        geo.rotate(0, dx, dy, center=origin.coords)
+        geo.update()
+
+
+def scale(event):  # type: (tkinter.Event) -> None
+    """ 缩放事件 """
+    k = 1.01 if event.delta > 0 else 0.99
+    for geo in geos:
+        geo.scale(k, k, k)
+        geo.update()
+
+
+root.bind('<Button-1>', lambda event: rotate(event, True))
+root.bind('<B1-Motion>', rotate)
+root.bind('<Button-3>', lambda event: translate(event, True))
+root.bind('<B3-Motion>', translate)
+root.bind('<MouseWheel>', scale)
+root.mainloop()
+```
+
+</details>
+
+更多更新信息请见：[CHANGELOG.md](./CHANGELOG.md)
+
 Description/模块说明
 ----------------------
 
 tkintertools 是一款基于 tkinter 模块的二次开发的界面编程模块，它完全没有使用任何第三方模块和库的，同时，它也没有任何依赖包，它的功能完全由内置模块和函数实现，而且，它还是跨平台的！它和 tkinter 最大的不同在于，它的控件并非真实的控件，而是在 tkinter 模块中 Canvas 对象中绘制而成的，这就赋予了 tkintertools 控件一些在 tkinter 中没有的特性，列举如下：
 
 * 控件背景可以是透明的（实际上是没有背景颜色）
 * 控件的样式可以是自定义的（比如按钮有圆角）
@@ -134,27 +243,27 @@
 见 [DPI 级别设置函数](#DPI)
 
 ### Detailed type hints/详细的类型提示
 
 参考 [PEP 526](https://peps.python.org/pep-0526/)、[PEP 586](https://peps.python.org/pep-0586/)、[PEP 604](https://peps.python.org/pep-0604/) 和 [PEP 612](https://peps.python.org/pep-0612/)，我采用了最兼容的方式去实现详细的类型提示，可适用 IDE 有 VScode、Pycharm 等。  
 那什么是类型提示呢？话不多说，直接看图就行：
 
-<p><img height="350px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/type_hint_vscode.png" alt="type_hint.png"/></p>
+![type_hint.png](docs/images/type_hint_vscode.png)
 
 在 VSCode 编辑器中，当鼠标移至类或者函数的名字上面时，会自动显示该类或者函数的注释文档。通过这种方式，不需要看太多的帮助文档和资料就能熟练地使用 tkintertools 模块！
 
 ### Across Platforms/跨平台
 
 [test.py](./test.py) 在 Windows 系统（Windows10）上运行的界面如下：
 
-<p><img height="383px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/test_win32.png" alt="test_win32.png"/></p>
+![test_win32.png](docs/images/test_win32.png)
 
 [test.py](./test.py) 在 Linux 系统（Ubuntu22.04）上运行的界面如下：
 
-<p><img height="408px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/test_linux.png" alt="test_linux.png"/></p>
+![test_linux.png](docs/images/test_linux.png)
 
 Contents/模块内容
 -------------------
 
 Each non internal class and function in the module will be described in detail here  
 这里会详细说明模块中的每个非内部类和函数
 
@@ -174,15 +283,16 @@
 
 ### Virtual Canvas Widget/虚拟画布控件
 
 1. `Label`: 标签控件
 
     标签控件的功能和`tkinter.Label`的功能类似，但更加的多元化  
     下面是`Label`控件的外观：  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/LabelTest.png" alt="LabelTest.png" /></p>
+
+    ![LabelTest.png](docs/images/LabelTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('LabelTest', 1000, 400)
@@ -207,16 +317,17 @@
     ```
 
     </details>
 
 2. `Button`: 按钮控件
 
     按钮控件相较于`tkinter.Button`，其自由度更高，`tkinter.Button`只有在按下的时候才能触发绑定的关联事件，而`Button`却可以在鼠标移至按钮上方时、鼠标按下时、鼠标松开时都可以绑定关联事件  
-    下面是`Button`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ButtonTest.png" alt="ButtonTest.png" /></p>
+    下面是`Button`控件的外观：
+
+    ![ButtonTest.png](docs/images/ButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ButtonTest', 500, 500)
@@ -242,15 +353,16 @@
 
     </details>
 
 3. `CheckButton`: 复选框控件
 
     复选框控件相对于`tkinter`原生的`tkinter.CheckButton`在使用方面更加地简单，同时颜值也上升了不少  
     下面是`CheckButton`控件的外观：
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/CheckButtonTest.png" alt="CheckButtonTest.png"/></p>
+
+    ![CheckButtonTest.png](docs/images/CheckButtonTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('CheckButtonTest', 500, 300)
@@ -276,16 +388,17 @@
     ```
 
     </details>
 
 4. `Entry`: 输入框控件
 
     输入框控件可以轻松地设置输入的文本位置（靠左、居中和靠右），同时，它可以在鼠标移至输入框上方、鼠标未在输入框上方两种状态显示不同的默认文本  
-    下面是`Entry`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/EntryTest.png" alt="EntryTest.png" /></p>
+    下面是`Entry`控件的外观：
+
+    ![EntryTest.png](docs/images/EntryTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('EntryTest', 500, 400)
@@ -321,16 +434,17 @@
     ```
 
     </details>
 
 5. `Text`: 文本框控件
 
     文本框类似于输入框，这里就不再赘述  
-    下面是`Text`控件的外观：  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/TextTest.png" alt="TextTest.png" /></p>
+    下面是`Text`控件的外观：
+
+    ![TextTest.png](docs/images/TextTest.png)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('TextTest', 1000, 400)
@@ -356,16 +470,17 @@
     ```
 
     </details>
 
 6. `Progressbar`: 进度条控件
 
     进度条控件相比`tkinter.ttk.Progressbar`，外观上的自由度较大  
-    下面是`Progressbar`控件的外观：  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ProgressbarTest.png" alt="ProgressbarTest.png" /></p>
+    下面是`Progressbar`控件的外观：
+
+    ![ProgressbarTest.png](docs/images/ProgressbarTest.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ProgressbarTest', 500, 500)
@@ -417,16 +532,17 @@
 
     单例模式，不用介绍了吧？通过继承它来使用
 
 ### Tool Function/工具函数
 
 1. `move`: <a name="move">移动函数</a>
 
-    移动函数可以轻松地按一定的规律、移动速度、移动时间去移动`tkintertools`模块内的所有对象，同时兼容了`tkinter`内的对象，即`tkinter`中的对象也可以很方便地移动，甚至它还可以移动窗口的位置！  
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/MoveTest.gif" alt="MoveTest.gif" /></p>
+    移动函数可以轻松地按一定的规律、移动速度、移动时间去移动`tkintertools`模块内的所有对象，同时兼容了`tkinter`内的对象，即`tkinter`中的对象也可以很方便地移动，甚至它还可以移动窗口的位置！
+
+    ![MoveTest.gif](docs/images/MoveTest.gif)
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('MoveTest', 500, 500)
@@ -470,17 +586,19 @@
     `left`   : "tkintertools        "  
     `center` : "    tkintertools    "  
     `right`  : "        tkintertools"</pre>
 
 3. `color`: <a name="Gradient">颜色函数</a>
 
     颜色函数可以轻松求出一个颜色到另外一个颜色的过渡颜色，因此可以轻松得到渐变色的效果，同时，改变传入的参数还可以得到传入颜色的对比色  
-    第二张图是 test.py 在图像测试中绘制的图案  
-    <p><img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/ColorTest.png" alt="ColorTest.png" />
-    <img width="360px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/Test_Draw.png" alt="Test_Draw.png" /></p>
+    第二张图是 test.py 在图像测试中绘制的图案
+
+    ![ColorTest.png](docs/images/ColorTest.png)
+
+    ![Test_Draw.png](docs/images/Test_Draw.png)
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ColorTest', 500, 500)
@@ -510,19 +628,19 @@
     <p><img width="540px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/font.png" alt="font.png" /></p>
 
 5. `SetProcessDpiAwareness`: <a name="DPI">DPI 级别设置函数</a>
 
     这个函数实际上只是对函数`ctypes.WinDLL('shcore').SetProcessDpiAwareness`的一个简单包装，其值可为 0、1 和 2，分别代表程序 DPI 的不同级别，那么缩放效果也就不同，`tkintertools`选择的值是 1，但程序默认值实际为 0  
     下面是未执行这个函数的效果
     
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/SetProcessDpiAwareness_0.png" alt="SetProcessDpiAwareness_0.png" /></p>
+    ![SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
 
     <p>下面是执行了这个函数的效果</p>
 
-    <p><img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/images/SetProcessDpiAwareness_1.png" alt="SetProcessDpiAwareness_1.png" /></p>
+    ![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
 
     从上面的两张图中可以很明显的看出第一张很模糊，第二张很清晰，这就是 DPI 级别不同的原因，不过这一点在屏幕缩放比不是 100% 的时候才会出现  
     大家对上面的图肯定很熟悉，这不就是 IDLE 吗！？对，这个的问题的解决办法也是来自于 IDLE 的源代码 [pyshell.py line 18~20]  
     注意：该函数在程序的不同位置执行的效果不一样！一般用在`mainloop`之前，但`tkintertools`已经在`mainloop`函数中嵌入了该函数，无需再设置一次 DPI 级别，此函数是为了原生`tkinter`程序用的。
 
 Examples/实战示例
 ----------------
@@ -565,25 +683,23 @@
 * 文章链接: 暂无
 * 代码仓库: https://gitcode.net/weixin_62651706/tester
 * 程序下载: 暂无
 * 推荐指数: 👍👍👍
 
 这个案例使用了最新稳定版的 tkintertools-v2.6.0，界面非常稳定，几乎没有 bug，完全采用 tkintertools 的控件，颜值很高，界面非常流畅。体现了 tkintertools 模块与 tkinter 模块相比在性能上的优越性！
 
-<p>
-    <img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/examples/exam3_1.png" alt="client.png"/>
-    <img width="720px" src="https://gitcode.net/weixin_62651706/tkintertools/-/raw/master/docs/examples/exam3_2.png" alt="client.png"/>
-</p>
+![exam3_1.png](docs/examples/exam3_1.png)
+![exam3_2.png](docs/examples/exam3_2.png)
 
 More/更多
 ---------
 
-> GitCode:  
-> https://gitcode.net/weixin_62651706/tkintertools
+> GitHub:  
+> https://github.com/Xiaokang2022/tkintertools
 
-> GitHub(Mirror/镜像):  
-> https://github.com/XiaoKang2022-CSDN/tkintertools
+> GitCode(Mirror/镜像):  
+> https://gitcode.net/weixin_62651706/tkintertools
 
-> Column/专栏:  
-> https://blog.csdn.net/weixin_62651706/category_11600888.html
+> Gitee(Mirror/镜像):  
+> https://gitee.com/xiaokang-2022/tkintertools
 
 还有更多内容请在 [源代码](./tkintertools/) 中探索！
```

#### html2text {}

```diff
@@ -1,33 +1,73 @@
-Metadata-Version: 2.1 Name: tkintertools Version: 2.6.1.2 Summary: An auxiliary
+Metadata-Version: 2.1 Name: tkintertools Version: 2.6.2 Summary: An auxiliary
 module of the tkinder module Home-page: https://gitcode.net/weixin_62651706/
 tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com License:
 MulanPSL-2.0 Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
                                   [logo.png]
      The tkintertools module is an auxiliary module of the tkinter module
              tkintertools æ¨¡åæ¯ tkinter æ¨¡åçè¾å©æ¨¡å
           [latest_version] [License] [ChangeLog] [ToDos] [Downloads]
                             [Email] [Blog] [Author]
 Installation/æ¨¡åå®è£ ----------------------- ### Stable version/
-ç¨³å®çæ¬ * Version/çæ¬ : 2.6.1 * Release Date/åå¸æ¥æ : 2023/05/21
-``` pip install tkintertools==2.6.1 ``` æè ``` pip install tkintertools ```
-è¿ä¸ªæ¯ç®åçææ°çï¼æ¯è¾ç¨³å®ï¼bug
+ç¨³å®çæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/30
+``` pip install tkintertools==2.6.2 ``` æè ``` pip install tkintertools ```
+è¿ä¸ªæ¯ç®åçææ°ç¨³å®çï¼æ¯è¾ç¨³å®ï¼bug
 æ²¡æé£ä¹å¤ï¼æ¨èä½¿ç¨è¿ä¸ªã ç¨³å®çæææ¡£å¯ä»¥æ¥çï¼æ
 issue æä¼å»æ¥çå¹¶å°è¯è§£å³ issueã ### Development version/
-å¼åçæ¬ * Version/çæ¬ : 2.6.1 * Release Date/åå¸æ¥æ : 2023/05/21
-``` pip install tkintertools-dev==2.6.1 ```
+å¼åçæ¬ * Version/çæ¬ : 2.6.2 * Release Date/åå¸æ¥æ : 2023/05/26
+``` pip install tkintertools-dev==2.6.2 ```
 è¿ä¸ªæ¯ä½èæ­£å¨å¼åççæ¬ï¼ææ°åè½ï¼ä½ä¸è½ä¿è¯ç¨³å®ï¼bug
 å¯è½ä¼æ¯è¾å¤ã å¼åçæ¬æ²¡æå¯¹åºçææ¡£ï¼å¤§å®¶å¯ä»¥å¨ issue
 ä¸­æåºå»ºè®®ï¼æä¼éå½éçº³ä¸äºå¹¶å¨å¼åçæ¬ä¸­æ´æ¹æå®ç°ã
-Description/æ¨¡åè¯´æ ---------------------- tkintertools æ¯ä¸æ¬¾åºäº
-tkinter
+News/ææ°åè½ -----------
+-
+ææ°çç`tkintertools`ä¸º`2.6.2`ï¼æ°å¢ä¸é¡¹æä¸ºå¼ºå¤§çåè½ï¼3dç»å¾ï¼
+åæ¶ä¿®å¤ä¸äºbugï¼ä¼åäºä¸é¨åä»£ç ï¼æåäºä¸é¨åæ§è½ã
+éè¿ä»¥ä¸ä»£ç æ¥ä½¿ç¨3dç»å¾åè½ï¼ ```python from tkintertools import
+tools_3d as t3d import tkintertools.tools_3d as t3d #
+ä¸¤ç§å¼å¥æ¹å¼é½å¯ä»¥ ``` å­æ¨¡å: [tools_3d.py](./tkintertools/
+tools_3d.py)
+ç®å3dç»å¾åè½è¿æ¯è¾ç®éï¼ä»è½ç»å¶ç¹ãçº¿ãé¢ä»¥åç´è¾¹çç©ºé´å ä½ä½ï¼å¯¹äºæ²è¾¹çç©ºé´å ä½ä½è¿å¨å¼åä¸­ï¼
+ä»¥ä¸æ¯ä¸ä¸ªä½¿ç¨3dç»å¾çç¤ºä¾ï¼
+å¨è¿ä¸ªç¤ºä¾ä¸­ï¼æä½é¼ æ å·¦é®å¯ä»¥æè½¬å ä½ä½ï¼æä½é¼ æ å³é®å¯ä»¥å¹³ç§»å ä½ä½ï¼æ»å¨é¼ æ æ»è½®å¯ä»¥ç¼©æ¾å ä½ä½ï¼
+xãy å z è½´åå«æ¯çº¢è²ãç»¿è²åèè²ççº¿ã ![3dç»å¾](./docs/
+images/3d.png) æºä»£ç  ```python import random import tkinter import
+tkintertools as tkt from tkintertools import tools_3d as t3d root = tkt.Tk
+('tools_3d', 1280, 720) canvas = t3d.Canvas_3D(root, 1280, 720, 0, 0) geos = []
+# type: list[t3d.Geometry] origin = t3d.Point(canvas, [0, 0, 0], size=5) #
+åç¹ axes = [t3d.Line(canvas, [0, 0, 0], [100, 0, 0], width=3, fill='red'), #
+åå»ºåæ è½´ t3d.Line(canvas, [0, 0, 0], [0, 100, 0], width=3,
+fill='green'), t3d.Line(canvas, [0, 0, 0], [0, 0, -100], width=3, fill='blue')]
+for _ in range(8): # åå»ºæ­£æ¹ä½ cube = t3d.Cuboid( canvas, *random.sample
+(range(-200, 200), 3), *random.sample(range(50, 100), 3)) geos.append(cube) #
+åå»ºåé¢ä½ x, y, z = random.sample(range(-200, 200), 3) tetr =
+t3d.Tetrahedron( canvas, *[[x+random.randint(-100, 100), y+random.randint(-100,
+100), z+random.randint(-100, 100)] for _ in range(4)]) geos.append(tetr) def
+translate(event, flag=False, _cache=[]): # type: (tkinter.Event, bool, list
+[float]) -> None """ å¹³ç§»äºä»¶ """ if flag: _cache[:] = [event.x, event.y]
+return dx = (event.x - _cache[0]) / 6 dy = (event.y - _cache[1]) / 6 _cache[:
+] = [event.x, event.y] for axis in axes: axis.translate(0, 6*dx, 6*dy)
+axis.update() for geo in geos: geo.translate(0, dx, dy) geo.update()
+origin.translate(0, 6*dx, 6*dy) origin.update() def rotate(event, flag=False,
+_cache=[]): # type: (tkinter.Event, bool, list[float]) -> None """ æè½¬äºä»¶
+""" if flag: _cache[:] = [event.x, event.y] return dy = (event.x - _cache[0]) /
+200 dx = (_cache[1] - event.y) / 200 _cache[:] = [event.x, event.y] for axis in
+axes: axis.rotate(0, 6*dx, 6*dy, center=origin.coords) axis.update() for geo in
+geos: geo.rotate(0, dx, dy, center=origin.coords) geo.update() def scale
+(event): # type: (tkinter.Event) -> None """ ç¼©æ¾äºä»¶ """ k = 1.01 if
+event.delta > 0 else 0.99 for geo in geos: geo.scale(k, k, k) geo.update()
+root.bind('', lambda event: rotate(event, True)) root.bind('', rotate)
+root.bind('', lambda event: translate(event, True)) root.bind('', translate)
+root.bind('', scale) root.mainloop() ```  æ´å¤æ´æ°ä¿¡æ¯è¯·è§ï¼
+[CHANGELOG.md](./CHANGELOG.md) Description/æ¨¡åè¯´æ ---------------------
+- tkintertools æ¯ä¸æ¬¾åºäº tkinter
 æ¨¡åçäºæ¬¡å¼åççé¢ç¼ç¨æ¨¡åï¼å®å®å¨æ²¡æä½¿ç¨ä»»ä½ç¬¬ä¸æ¹æ¨¡åååºçï¼åæ¶ï¼å®ä¹æ²¡æä»»ä½ä¾èµåï¼å®çåè½å®å¨ç±åç½®æ¨¡ååå½æ°å®ç°ï¼èä¸ï¼å®è¿æ¯è·¨å¹³å°çï¼å®å
 tkinter æå¤§çä¸åå¨äºï¼å®çæ§ä»¶å¹¶éçå®çæ§ä»¶ï¼èæ¯å¨
 tkinter æ¨¡åä¸­ Canvas å¯¹è±¡ä¸­ç»å¶èæçï¼è¿å°±èµäºäº
 tkintertools æ§ä»¶ä¸äºå¨ tkinter ä¸­æ²¡æçç¹æ§ï¼åä¸¾å¦ä¸ï¼ *
 æ§ä»¶èæ¯å¯ä»¥æ¯éæçï¼å®éä¸æ¯æ²¡æèæ¯é¢è²ï¼ *
 æ§ä»¶çæ ·å¼å¯ä»¥æ¯èªå®ä¹çï¼æ¯å¦æé®æåè§ï¼ *
 æ§ä»¶çåå»ºéåº¦è¿å¤§äº tkinter çæ§ä»¶ï¼é¤äº Canvas æ§ä»¶ï¼
@@ -58,78 +98,71 @@
 (#Gradient) ### Automatically adapt to DPI/èªå¨éåºDPI è§ [DPI
 çº§å«è®¾ç½®å½æ°](#DPI) ### Detailed type hints/è¯¦ç»çç±»åæç¤º åè
 [PEP 526](https://peps.python.org/pep-0526/)ã[PEP 586](https://
 peps.python.org/pep-0586/)ã[PEP 604](https://peps.python.org/pep-0604/) å
 [PEP 612](https://peps.python.org/pep-0612/
 )ï¼æéç¨äºæå¼å®¹çæ¹å¼å»å®ç°è¯¦ç»çç±»åæç¤ºï¼å¯éç¨
 IDE æ VScodeãPycharm ç­ã
-é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼
-[type_hint.png]
-å¨ VSCode
+é£ä»ä¹æ¯ç±»åæç¤ºå¢ï¼è¯ä¸å¤è¯´ï¼ç´æ¥çå¾å°±è¡ï¼ !
+[type_hint.png](docs/images/type_hint_vscode.png) å¨ VSCode
 ç¼è¾å¨ä¸­ï¼å½é¼ æ ç§»è³ç±»æèå½æ°çåå­ä¸é¢æ¶ï¼ä¼èªå¨æ¾ç¤ºè¯¥ç±»æèå½æ°çæ³¨éææ¡£ãéè¿è¿ç§æ¹å¼ï¼ä¸éè¦çå¤ªå¤çå¸®å©ææ¡£åèµæå°±è½çç»å°ä½¿ç¨
 tkintertools æ¨¡åï¼ ### Across Platforms/è·¨å¹³å° [test.py](./test.py) å¨
-Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼
-[test_win32.png]
-[test.py](./test.py) å¨ Linux
-ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼
-[test_linux.png]
-Contents/æ¨¡ååå®¹ ------------------- Each non internal class and function
-in the module will be described in detail here
+Windows ç³»ç»ï¼Windows10ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_win32.png]
+(docs/images/test_win32.png) [test.py](./test.py) å¨ Linux
+ç³»ç»ï¼Ubuntu22.04ï¼ä¸è¿è¡ççé¢å¦ä¸ï¼ ![test_linux.png](docs/
+images/test_linux.png) Contents/æ¨¡ååå®¹ ------------------- Each non
+internal class and function in the module will be described in detail here
 è¿éä¼è¯¦ç»è¯´ææ¨¡åä¸­çæ¯ä¸ªéåé¨ç±»åå½æ° ### Container
 Widget/å®¹å¨æ§ä»¶ 1. `Tk`: çªå£ç±»
 ç»§æ¿äº`tkinter.Tk`ï¼å¨ç»§æ¿äº`tkinter`æ¨¡åå`Tk`çåºç¡ä¸ï¼åå å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¹¶å å¥äºæ£æµçªå£å¤§å°æ¯å¦ç¼©æ¾çæºå¶ï¼ä»¥ä½¿å¾å¶å­`Canvas`åè½æ­£ç¡®å°è¿è¡ç¼©æ¾
 2. `Toplevel`: é¡¶çº§çªå£ç±»
 ç»§æ¿äº`tkinter.Toplevel`å`Tk`ï¼å å¥äºå¯¹`tkintertools`æ¨¡åä¸­ç`Canvas`å¯¹è±¡çæ¯æï¼å¶ä½åä¸`Tk`ä¸æ ·
 3. `Canvas`: ç»å¸ç±»
 ç»§æ¿äº`tkinter.Canvas`ï¼å å¥äºå¯¹ç»å¸èææ§ä»¶çæ¯æï¼åæ¶æ¯åç±»ååºäºä»¶ãç¼©æ¾æ§å¶çç®¡çèï¼ä¹å¯¹`tkinter.Canvas`çå®ä¾æ¹æ³æä¸å®çå¼å®¹æ§
 ### Virtual Canvas Widget/èæç»å¸æ§ä»¶ 1. `Label`: æ ç­¾æ§ä»¶
 æ ç­¾æ§ä»¶çåè½å`tkinter.Label`çåè½ç±»ä¼¼ï¼ä½æ´å çå¤åå
-ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼
-[LabelTest.png]
+ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼ ![LabelTest.png](docs/images/LabelTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('LabelTest', 1000,
 400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Label(canvas, 50, 50, 400, 100, text='NormalLabel\nHere is the text')
 tkt.Label(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerLabel')
 tkt.Label(canvas, 550, 50, 400, 100, text='DisableLabel').set_live(False)
 tkt.Label(canvas, 550, 200, 400, 100, radius=20, text='TransparentLabel',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  2. `Button`: æé®æ§ä»¶
 æé®æ§ä»¶ç¸è¾äº`tkinter.Button`ï¼å¶èªç±åº¦æ´é«ï¼`tkinter.Button`åªæå¨æä¸çæ¶åæè½è§¦åç»å®çå³èäºä»¶ï¼è`Button`å´å¯ä»¥å¨é¼ æ ç§»è³æé®ä¸æ¹æ¶ãé¼ æ æä¸æ¶ãé¼ æ æ¾å¼æ¶é½å¯ä»¥ç»å®å³èäºä»¶
-ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼
-[ButtonTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ButtonTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
-height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
-range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼ ![ButtonTest.png](docs/images/
+ButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk
+('ButtonTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful
+(x, y, width, height): # type: (int, int, int, int) -> None """ Gradient colors
+""" for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 280, 400,
 100) tkt.Button(canvas, 150, 135, 200, 50, text='NormalButton') tkt.Button
 (canvas, 100, 195, 300, 50, radius=10, text='RoundCornerButton') tkt.Button
 (canvas, 150, 255, 200, 50, text='DisableButton').set_live(False) tkt.Button
 (canvas, 100, 315, 300, 50, radius=10, text='TransparentButton',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  3. `CheckButton`:
 å¤éæ¡æ§ä»¶
 å¤éæ¡æ§ä»¶ç¸å¯¹äº`tkinter`åçç`tkinter.CheckButton`å¨ä½¿ç¨æ¹é¢æ´å å°ç®åï¼åæ¶é¢å¼ä¹ä¸åäºä¸å°
-ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼
-[CheckButtonTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('CheckButtonTest',
-500, 300) canvas = tkt.Canvas(root, 500, 300, 0, 0) def colorful(x, y, width,
-height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
-range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
-canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(40, 190, 420,
-50) tkt.CheckButton(canvas, 50, 50, 30, text='NormalCheckButton', value=True)
-tkt.CheckButton(canvas, 50, 100, 30, text='DisableCheckButton',
-value=True).set_live(False) tkt.CheckButton(canvas, 50, 150, 30, radius=10,
-text='RoundCornerCheckButton') tkt.CheckButton(canvas, 50, 200, 30, radius=15,
-text='TransparentCheckButton', color_fill=tkt.COLOR_NONE) root.mainloop() ```
-4. `Entry`: è¾å¥æ¡æ§ä»¶
+ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼ ![CheckButtonTest.png](docs/images/
+CheckButtonTest.png) æºä»£ç  ```python import tkintertools as tkt root =
+tkt.Tk('CheckButtonTest', 500, 300) canvas = tkt.Canvas(root, 500, 300, 0, 0)
+def colorful(x, y, width, height): # type: (int, int, int, int) -> None """
+Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
+'#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
+colorful(40, 190, 420, 50) tkt.CheckButton(canvas, 50, 50, 30,
+text='NormalCheckButton', value=True) tkt.CheckButton(canvas, 50, 100, 30,
+text='DisableCheckButton', value=True).set_live(False) tkt.CheckButton(canvas,
+50, 150, 30, radius=10, text='RoundCornerCheckButton') tkt.CheckButton(canvas,
+50, 200, 30, radius=15, text='TransparentCheckButton',
+color_fill=tkt.COLOR_NONE) root.mainloop() ```  4. `Entry`: è¾å¥æ¡æ§ä»¶
 è¾å¥æ¡æ§ä»¶å¯ä»¥è½»æ¾å°è®¾ç½®è¾å¥çææ¬ä½ç½®ï¼é å·¦ãå±ä¸­åé å³ï¼ï¼åæ¶ï¼å®å¯ä»¥å¨é¼ æ ç§»è³è¾å¥æ¡ä¸æ¹ãé¼ æ æªå¨è¾å¥æ¡ä¸æ¹ä¸¤ç§ç¶ææ¾ç¤ºä¸åçé»è®¤ææ¬
-ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼
-[EntryTest.png]
+ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼ ![EntryTest.png](docs/images/EntryTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('EntryTest', 500,
 400) canvas = tkt.Canvas(root, 500, 400, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 193, 400,
 100) tkt.Entry(canvas, 20, 20, 200, 30, text=('LeftEntry', 'Enter')) tkt.Entry
 (canvas, 20, 55, 200, 30, text=( 'CenterEntry', 'Enter'), justify='center')
@@ -140,79 +173,77 @@
 radius=8, text='RightEntry', justify='right') tkt.Entry(canvas, 100, 150, 300,
 35, text=('PasswordEntry', 'Click To Enter'), justify='center', show='â')
 tkt.Entry(canvas, 100, 200, 300, 35, text='DisableEntry',
 justify='center').set_live(False) tkt.Entry(canvas, 100, 250, 300, 35,
 text='TransparentEntry', justify='center', color_fill=tkt.COLOR_NONE)
 root.mainloop() ```  5. `Text`: ææ¬æ¡æ§ä»¶
 ææ¬æ¡ç±»ä¼¼äºè¾å¥æ¡ï¼è¿éå°±ä¸åèµè¿°
-ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼
-[TextTest.png]
+ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼ ![TextTest.png](docs/images/TextTest.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('TextTest', 1000,
 400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
 height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
 for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Text(canvas, 50, 50, 400, 100, text=('NormalText(Left)', 'Click To
 Enter')) tkt.Text(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerText
 (Center)', justify='center') tkt.Text(canvas, 550, 50, 400, 100,
 text='DisableText').set_live(False) tkt.Text(canvas, 550, 200, 400, 100,
 radius=20, text='TransparentText(Right)', justify='right',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  6. `Progressbar`:
 è¿åº¦æ¡æ§ä»¶
 è¿åº¦æ¡æ§ä»¶ç¸æ¯`tkinter.ttk.Progressbar`ï¼å¤è§ä¸çèªç±åº¦è¾å¤§
-ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼
-[ProgressbarTest.png]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ProgressbarTest',
-500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
-height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
-for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
-canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(30, 290, 440,
-50) tkt.Progressbar(canvas, 50, 50, 400, 30) tkt.Progressbar(canvas, 50, 100,
-400, 30).load(.6667) tkt.Progressbar(canvas, 50, 150, 400, 30,
-borderwidth=5).load(1) (_ := tkt.Progressbar(canvas, 50, 200, 400, 30)).load
-(0.3333) _.set_live(False) tkt.Progressbar(canvas, 50, 250, 400, 30, color_bar=
-( 'lightyellow', 'skyblue')).load(.5) tkt.Progressbar(canvas, 50, 300, 400, 30,
-color_bar=('', 'orange')).load(.1667) progressbar = tkt.Progressbar(canvas, 50,
-375, 400, 30) progressbar_2 = tkt.Progressbar(canvas, 50, 425, 400, 30) def
-load(total, count=0): # type: (int, int) -> None """ load progressbar """
-progressbar.load(count/total) progressbar_2.load(1-count/total) if count <
-total: root.after(3, load, total, count+1) load(10000) root.mainloop() ```  ###
-Tool Class/å·¥å·ç±» 1. `PhotoImage`: å¾çç±»
+ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼ ![ProgressbarTest.png](docs/images/
+ProgressbarTest.png) æºä»£ç  ```python import tkintertools as tkt root =
+tkt.Tk('ProgressbarTest', 500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0)
+def colorful(x, y, width, height) -> None: # type: (int, int, int, int) -> None
+""" Gradient colors """ for i in range(width): color = tkt.color(('#FF0000',
+'#0000FF'), i/width) canvas.create_line(x+i, y, x+i, y+height, fill=color)
+colorful(30, 290, 440, 50) tkt.Progressbar(canvas, 50, 50, 400, 30)
+tkt.Progressbar(canvas, 50, 100, 400, 30).load(.6667) tkt.Progressbar(canvas,
+50, 150, 400, 30, borderwidth=5).load(1) (_ := tkt.Progressbar(canvas, 50, 200,
+400, 30)).load(0.3333) _.set_live(False) tkt.Progressbar(canvas, 50, 250, 400,
+30, color_bar=( 'lightyellow', 'skyblue')).load(.5) tkt.Progressbar(canvas, 50,
+300, 400, 30, color_bar=('', 'orange')).load(.1667) progressbar =
+tkt.Progressbar(canvas, 50, 375, 400, 30) progressbar_2 = tkt.Progressbar
+(canvas, 50, 425, 400, 30) def load(total, count=0): # type: (int, int) -> None
+""" load progressbar """ progressbar.load(count/total) progressbar_2.load(1-
+count/total) if count < total: root.after(3, load, total, count+1) load(10000)
+root.mainloop() ```  ### Tool Class/å·¥å·ç±» 1. `PhotoImage`: å¾çç±»
 `PhotoImage`ç±»ç»§æ¿äº`tkinter.PhotoImage`ï¼å®æ¯å¨`tkinter.PhotoImage`çåºç¡ä¸ååè½çå¼ºåï¼å¯¹
 gif
 å¨å¾æå¾å¥½çæ¯æï¼ä»éæå°éä»£ç å³å¯å®ç°å¨å¾çæ¾ç¤ºï¼è¿å¯ä»¥è®¾ç½®å¨å¾æ¾ç¤ºçéåº¦ï¼æ­¤å¤ï¼å¯¹
 png
 ç±»åçå¾ççæ¯æä¹æå¼ºåï¼å¯ä»¥å¨ä¸ä¾èµä»»ä½ç¬¬ä¸æ¹æ¨¡åæèåºçæåµä¸ï¼å¯¹
 png å¾çè¿è¡ç¼©æ¾ 2. `Singleton`: åä¾æ¨¡å¼ç±»
 åä¾æ¨¡å¼ï¼ä¸ç¨ä»ç»äºå§ï¼éè¿ç»§æ¿å®æ¥ä½¿ç¨ ### Tool Function/
 å·¥å·å½æ° 1. `move`: ç§»å¨å½æ°
 ç§»å¨å½æ°å¯ä»¥è½»æ¾å°æä¸å®çè§å¾ãç§»å¨éåº¦ãç§»å¨æ¶é´å»ç§»å¨`tkintertools`æ¨¡ååçææå¯¹è±¡ï¼åæ¶å¼å®¹äº`tkinter`åçå¯¹è±¡ï¼å³`tkinter`ä¸­çå¯¹è±¡ä¹å¯ä»¥å¾æ¹ä¾¿å°ç§»å¨ï¼çè³å®è¿å¯ä»¥ç§»å¨çªå£çä½ç½®ï¼
-[MoveTest.gif]
-æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('MoveTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500, 0, 0) rect = canvas.create_rectangle
-(50, 350, 150, 450) def move_window(switch=[True]): # type: (list[bool]) -
-> None tkt.move(root, None, 1000 if switch[0] else -1000, 0, 800, mode='flat')
-switch[0] = not switch[0] def move_button(switch=[True]) -> None: # type: (list
-[bool]) -> None tkt.move(canvas, button, 200 if switch[0] else -200, 0, 500,
-mode='rebound') switch[0] = not switch[0] def move_rect(switch=[True]): # type:
-(list[bool]) -> None tkt.move(canvas, rect, 200 if switch[0] else -200, 0, 500,
-mode='smooth') switch[0] = not switch[0] tkt.Button(canvas, 50, 50, 200, 40,
-radius=10, text='MoveWindow', command=move_window) tkt.Button(canvas, 50, 100,
-200, 40, radius=10, text='MoveRect', command=move_rect) button = tkt.Button
-(canvas, 50, 150, 200, 40, radius=10, text='MoveButton', command=move_button)
-root.mainloop() ```  2. `text`: ææ¬å½æ°
+![MoveTest.gif](docs/images/MoveTest.gif) æºä»£ç  ```python import
+tkintertools as tkt root = tkt.Tk('MoveTest', 500, 500) canvas = tkt.Canvas
+(root, 500, 500, 0, 0) rect = canvas.create_rectangle(50, 350, 150, 450) def
+move_window(switch=[True]): # type: (list[bool]) -> None tkt.move(root, None,
+1000 if switch[0] else -1000, 0, 800, mode='flat') switch[0] = not switch[0]
+def move_button(switch=[True]) -> None: # type: (list[bool]) -> None tkt.move
+(canvas, button, 200 if switch[0] else -200, 0, 500, mode='rebound') switch[0]
+= not switch[0] def move_rect(switch=[True]): # type: (list[bool]) -> None
+tkt.move(canvas, rect, 200 if switch[0] else -200, 0, 500, mode='smooth')
+switch[0] = not switch[0] tkt.Button(canvas, 50, 50, 200, 40, radius=10,
+text='MoveWindow', command=move_window) tkt.Button(canvas, 50, 100, 200, 40,
+radius=10, text='MoveRect', command=move_rect) button = tkt.Button(canvas, 50,
+150, 200, 40, radius=10, text='MoveButton', command=move_button) root.mainloop
+() ```  2. `text`: ææ¬å½æ°
 å¯ä»¥å¿«éå¹¶æ¹ä¾¿å°å¾å°ä¸ä¸ªåæ°é¿åº¦çå­ç¬¦ä¸²ï¼ä¸å­ç¬¦ä¸²çåå®¹å¯ä»¥æå®ä½ç½®
 å¦ï¼å¾å°ä¸ä¸ª 20 é¿åº¦çå­ç¬¦ä¸² âtkintertoolsâ
     `left`   : "tkintertools        "
     `center` : "    tkintertools    "
     `right`  : "        tkintertools"
 3. `color`: é¢è²å½æ°
 é¢è²å½æ°å¯ä»¥è½»æ¾æ±åºä¸ä¸ªé¢è²å°å¦å¤ä¸ä¸ªé¢è²çè¿æ¸¡é¢è²ï¼å æ­¤å¯ä»¥è½»æ¾å¾å°æ¸åè²çææï¼åæ¶ï¼æ¹åä¼ å¥çåæ°è¿å¯ä»¥å¾å°ä¼ å¥é¢è²çå¯¹æ¯è²
-ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡
-[ColorTest.png] [Test_Draw.png]
+ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡ ![ColorTest.png]
+(docs/images/ColorTest.png) ![Test_Draw.png](docs/images/Test_Draw.png)
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ColorTest', 500,
 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 =
 tkt.color(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i,
 y+height, fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
 outline=color_2, width=2) colorful(50, 50, 400, 100) root.mainloop() ```  4.
@@ -222,18 +253,18 @@
 tcl çå½ä»¤ï¼ä½¿å¾å­ä½éæ©æ¡è½å¤è¢«æä»¬ä½¿ç¨ã
 [font.png]
 5. `SetProcessDpiAwareness`: DPI çº§å«è®¾ç½®å½æ°
 è¿ä¸ªå½æ°å®éä¸åªæ¯å¯¹å½æ°`ctypes.WinDLL
 ('shcore').SetProcessDpiAwareness`çä¸ä¸ªç®ååè£ï¼å¶å¼å¯ä¸º 0ã1
 å 2ï¼åå«ä»£è¡¨ç¨åº DPI
 çä¸åçº§å«ï¼é£ä¹ç¼©æ¾ææä¹å°±ä¸åï¼`tkintertools`éæ©çå¼æ¯
-1ï¼ä½ç¨åºé»è®¤å¼å®éä¸º 0 ä¸é¢æ¯æªæ§è¡è¿ä¸ªå½æ°çææ
-[SetProcessDpiAwareness_0.png]
+1ï¼ä½ç¨åºé»è®¤å¼å®éä¸º 0 ä¸é¢æ¯æªæ§è¡è¿ä¸ªå½æ°çææ !
+[SetProcessDpiAwareness_0.png](docs/images/SetProcessDpiAwareness_0.png)
 ä¸é¢æ¯æ§è¡äºè¿ä¸ªå½æ°çææ
-[SetProcessDpiAwareness_1.png]
+![SetProcessDpiAwareness_1.png](docs/images/SetProcessDpiAwareness_1.png)
 ä»ä¸é¢çä¸¤å¼ å¾ä¸­å¯ä»¥å¾ææ¾ççåºç¬¬ä¸å¼ å¾æ¨¡ç³ï¼ç¬¬äºå¼ å¾æ¸æ°ï¼è¿å°±æ¯
 DPI çº§å«ä¸åçåå ï¼ä¸è¿è¿ä¸ç¹å¨å±å¹ç¼©æ¾æ¯ä¸æ¯ 100%
 çæ¶åæä¼åºç° å¤§å®¶å¯¹ä¸é¢çå¾è¯å®å¾çæï¼è¿ä¸å°±æ¯ IDLE
 åï¼ï¼å¯¹ï¼è¿ä¸ªçé®é¢çè§£å³åæ³ä¹æ¯æ¥èªäº IDLE çæºä»£ç 
 [pyshell.py line 18~20]
 æ³¨æï¼è¯¥å½æ°å¨ç¨åºçä¸åä½ç½®æ§è¡çææä¸ä¸æ ·ï¼ä¸è¬ç¨å¨`mainloop`ä¹åï¼ä½`tkintertools`å·²ç»å¨`mainloop`å½æ°ä¸­åµå¥äºè¯¥å½æ°ï¼æ éåè®¾ç½®ä¸æ¬¡
 DPI çº§å«ï¼æ­¤å½æ°æ¯ä¸ºäºåç`tkinter`ç¨åºç¨çã Examples/
@@ -262,14 +293,13 @@
 æ¨¡åçå¼å®¹æ§ï¼
 [chess.png] [chess.png]
 ### ç®æç»å½çé¢ * æç« é¾æ¥: ææ  * ä»£ç ä»åº: https://
 gitcode.net/weixin_62651706/tester * ç¨åºä¸è½½: ææ  * æ¨èææ°:
 ððð è¿ä¸ªæ¡ä¾ä½¿ç¨äºææ°ç¨³å®çç tkintertools-
 v2.6.0ï¼çé¢éå¸¸ç¨³å®ï¼å ä¹æ²¡æ bugï¼å®å¨éç¨ tkintertools
 çæ§ä»¶ï¼é¢å¼å¾é«ï¼çé¢éå¸¸æµçãä½ç°äº tkintertools
-æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼
-[client.png] [client.png]
-More/æ´å¤ --------- > GitCode: > https://gitcode.net/weixin_62651706/
-tkintertools > GitHub(Mirror/éå): > https://github.com/XiaoKang2022-CSDN/
-tkintertools > Column/ä¸æ : > https://blog.csdn.net/weixin_62651706/
-category_11600888.html è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/
-) ä¸­æ¢ç´¢ï¼
+æ¨¡åä¸ tkinter æ¨¡åç¸æ¯å¨æ§è½ä¸çä¼è¶æ§ï¼ ![exam3_1.png](docs/
+examples/exam3_1.png) ![exam3_2.png](docs/examples/exam3_2.png) More/æ´å¤ ---
+------ > GitHub: > https://github.com/Xiaokang2022/tkintertools > GitCode
+(Mirror/éå): > https://gitcode.net/weixin_62651706/tkintertools > Gitee
+(Mirror/éå): > https://gitee.com/xiaokang-2022/tkintertools
+è¿ææ´å¤åå®¹è¯·å¨ [æºä»£ç ](./tkintertools/) ä¸­æ¢ç´¢ï¼
```

