# Comparing `tmp/pdocr_rpc-1.1.3.tar.gz` & `tmp/pdocr_rpc-1.1.4.tar.gz`

## Comparing `pdocr_rpc-1.1.3.tar` & `pdocr_rpc-1.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/pdocr_rpc/__init__.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/pdocr_rpc/__version__.py
--rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/pdocr_rpc/ocr.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/pdocr_rpc/ocr_server.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/pdocr_rpc/setting.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/LICENSE
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.4/pdocr_rpc/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.4/pdocr_rpc/__version__.py
+-rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.4/pdocr_rpc/ocr.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.4/pdocr_rpc/ocr_server.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.4/pdocr_rpc/setting.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.4/LICENSE
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.4/README.md
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.4/PKG-INFO
```

### Comparing `pdocr_rpc-1.1.3/pdocr_rpc/ocr.py` & `pdocr_rpc-1.1.4/pdocr_rpc/ocr.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-1.1.3/pdocr_rpc/ocr_server.py` & `pdocr_rpc-1.1.4/pdocr_rpc/ocr_server.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-1.1.3/pdocr_rpc/setting.py` & `pdocr_rpc-1.1.4/pdocr_rpc/setting.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-1.1.3/LICENSE` & `pdocr_rpc-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-1.1.3/README.md` & `pdocr_rpc-1.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,45 +2,24 @@
 
 基于 `PaddleOCR` 封装的 `RPC` 服务，包含客户端和服务端。
 
 客户端提供了一个简单易用的函数 `ocr`，通过不同的参数控制返回不同的值。
 
 Documents：https://funny-test.github.io/pdocr-rpc
 
-## 1、安装
+## 1、客户端安装
 
 ```shell
 pip install pdocr-rpc
 ```
 
-另外还需要手动安装以下依赖：
+### 1.2、服务端安装
 
-### 1.1、客户端依赖
-
-客户端仅需要安装**截图工具**；
-
-- `Windows` 上安装截图工具：
-
-  ```shell
-  pip3 install pillow
-  ```
-
-- `Linux` 上安装截图工具：
-
-```console
-pip3 install pyscreenshot
-```
-
-### 1.2、服务端依赖
-
-安装 `PaddleOCR` 环境：
-
-```console
-pip3 install paddlepaddle -i https://mirror.baidu.com/pypi/simple
-pip3 install "paddleocr>=2.0.1" -i https://mirror.baidu.com/pypi/simple
+```shell
+pip install pdocr-rpc[server]
 ```
 
 ## 2、使用方法
 
 ### 2.1、服务端
 
 随意新建一个`py`文件，比如：`ocr_server.py`；
@@ -51,15 +30,15 @@
 # ocr_server.py
 from pdocr_rpc.ocr_server import ocr_server
 
 if __name__ == '__main__':
     ocr_server()
 ```
 
-如果你想修改端口：
+默认端口号为 `8890` 如果你想修改端口：
 
 ```python
 from pdocr_rpc.ocr_server import ocr_server
 from pdocr_rpc.setting import setting
 
 setting.PORT = 8888
 
@@ -68,83 +47,88 @@
 ```
 
 ### 2.2、客户端
 
 #### 2.1、识别当前屏幕的所有文字内容
 
 ```python
-from pdocr_rpc.ocr import ocr
+from pdocr_rpc.ocr import OCR
+from pdocr_rpc.setting import setting
+
+# 注意IP和端口要和你的服务端IP对应
+setting.SERVER_IP = "192.168.0.1"
+setting.PORT = 8888
 
-ocr()
+OCR.ocr()
 ```
 
 自动识别当前整个屏幕的所有内容。
 
 #### 2.2、指定某张图片识别的所有文字内容
 
 ```python
-ocr(picture_abspath="~/Desktop/test.png")
+OCR.ocr(picture_abspath="~/Desktop/test.png")
 ```
 
 返回识别图片 `test.png` 的内容。 
 
 #### 2.3、在全屏指定查找某个字符串的坐标
 
 ```python
-ocr("天天向上")
+OCR.ocr("天天向上")
 ```
 
 返回当前屏幕中，“天天向上”的坐标，如果存在多个，则返回一个字典。
 
 #### 2.4、指定某张图片查找某个字符串的坐标
 
 ```python
-ocr("天天向上"，picture_abspath="~/Desktop/test.png")
+OCR.ocr("天天向上"，picture_abspath="~/Desktop/test.png")
 ```
 
 #### 2.5、其他参数
 
 - 识别语言
 
   lang： `ch`, `en`, `fr`, `german`, `korean`, `japan`
 
   默认为ch，中文，如果要修改识别语言；
 
   ```python
-  ocr(lang="ch") 
+  OCR.ocr(lang="ch") 
   ```
 
 - 匹配度
 
   similarity: float
 
   默认为0.6，可以修改为从0到1的数；
 
   ```shell
-  ocr(similarity=0.1)
+  OCR.ocr(similarity=0.1)
   ```
 
 - 返回原始数据
 
   return_default: bool
 
   默认为False，即默认返回识别到字符串的中心坐标，True表示返回原始数据；
 
   ```python
-  ocr(return_default=False)
+  OCR.ocr(return_default=False)
   ```
 
 - 只返回第一个
 
   return_first: bool
 
   当传入要查找的字符串时，可能存在当前屏幕中有多个目标；
 
   默认情况下是会将识别到的多个目标组装成字典返回；
 
   return_first=True 表示返回识别到的第一个。
 
   ```python
-  ocr(return_first=True )
+  OCR.ocr(return_first=True )
   ```
```

### Comparing `pdocr_rpc-1.1.3/pyproject.toml` & `pdocr_rpc-1.1.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -13,23 +13,38 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "pyscreenshot",
+    "pyscreenshot;sys_platform == 'linux'",
+    "pillow;sys_platform == 'win32'",
 ]
+
+
 dynamic = ["version"]
 
+[project.optional-dependencies]
+server = [
+    "paddlepaddle",
+    "paddleocr>=2.0.1"
+]
+
+test = [
+    "pytest",
+]
+
+doc = ["mkdocs-material"]
+
 [tool.hatch.version]
 path = "pdocr_rpc/__version__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "/pdocr_rpc",
     "/README.md",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/funny-test/pdocr-rpc"
-"Bug Tracker" = "https://github.com/funny-test/pdocr-rpc/issues"
+Source = "https://github.com/funny-test/pdocr-rpc"
+Documentation = "https://funny-test.github.io/pdocr-rpc"
```

### Comparing `pdocr_rpc-1.1.3/PKG-INFO` & `pdocr_rpc-1.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 Metadata-Version: 2.1
 Name: pdocr-rpc
-Version: 1.1.3
+Version: 1.1.4
 Summary: PaddleOCR-RPC
-Project-URL: Homepage, https://github.com/funny-test/pdocr-rpc
-Project-URL: Bug Tracker, https://github.com/funny-test/pdocr-rpc/issues
+Project-URL: Source, https://github.com/funny-test/pdocr-rpc
+Project-URL: Documentation, https://funny-test.github.io/pdocr-rpc
 Author-email: mikigo <1964191531@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: pyscreenshot
+Requires-Dist: pillow; sys_platform == 'win32'
+Requires-Dist: pyscreenshot; sys_platform == 'linux'
+Provides-Extra: doc
+Requires-Dist: mkdocs-material; extra == 'doc'
+Provides-Extra: server
+Requires-Dist: paddleocr>=2.0.1; extra == 'server'
+Requires-Dist: paddlepaddle; extra == 'server'
+Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 # pdocr-rpc
 
 基于 `PaddleOCR` 封装的 `RPC` 服务，包含客户端和服务端。
 
 客户端提供了一个简单易用的函数 `ocr`，通过不同的参数控制返回不同的值。
 
 Documents：https://funny-test.github.io/pdocr-rpc
 
-## 1、安装
+## 1、客户端安装
 
 ```shell
 pip install pdocr-rpc
 ```
 
-另外还需要手动安装以下依赖：
+### 1.2、服务端安装
 
-### 1.1、客户端依赖
-
-客户端仅需要安装**截图工具**；
-
-- `Windows` 上安装截图工具：
-
-  ```shell
-  pip3 install pillow
-  ```
-
-- `Linux` 上安装截图工具：
-
-```console
-pip3 install pyscreenshot
-```
-
-### 1.2、服务端依赖
-
-安装 `PaddleOCR` 环境：
-
-```console
-pip3 install paddlepaddle -i https://mirror.baidu.com/pypi/simple
-pip3 install "paddleocr>=2.0.1" -i https://mirror.baidu.com/pypi/simple
+```shell
+pip install pdocr-rpc[server]
 ```
 
 ## 2、使用方法
 
 ### 2.1、服务端
 
 随意新建一个`py`文件，比如：`ocr_server.py`；
@@ -66,15 +53,15 @@
 # ocr_server.py
 from pdocr_rpc.ocr_server import ocr_server
 
 if __name__ == '__main__':
     ocr_server()
 ```
 
-如果你想修改端口：
+默认端口号为 `8890` 如果你想修改端口：
 
 ```python
 from pdocr_rpc.ocr_server import ocr_server
 from pdocr_rpc.setting import setting
 
 setting.PORT = 8888
 
@@ -83,83 +70,88 @@
 ```
 
 ### 2.2、客户端
 
 #### 2.1、识别当前屏幕的所有文字内容
 
 ```python
-from pdocr_rpc.ocr import ocr
+from pdocr_rpc.ocr import OCR
+from pdocr_rpc.setting import setting
+
+# 注意IP和端口要和你的服务端IP对应
+setting.SERVER_IP = "192.168.0.1"
+setting.PORT = 8888
 
-ocr()
+OCR.ocr()
 ```
 
 自动识别当前整个屏幕的所有内容。
 
 #### 2.2、指定某张图片识别的所有文字内容
 
 ```python
-ocr(picture_abspath="~/Desktop/test.png")
+OCR.ocr(picture_abspath="~/Desktop/test.png")
 ```
 
 返回识别图片 `test.png` 的内容。 
 
 #### 2.3、在全屏指定查找某个字符串的坐标
 
 ```python
-ocr("天天向上")
+OCR.ocr("天天向上")
 ```
 
 返回当前屏幕中，“天天向上”的坐标，如果存在多个，则返回一个字典。
 
 #### 2.4、指定某张图片查找某个字符串的坐标
 
 ```python
-ocr("天天向上"，picture_abspath="~/Desktop/test.png")
+OCR.ocr("天天向上"，picture_abspath="~/Desktop/test.png")
 ```
 
 #### 2.5、其他参数
 
 - 识别语言
 
   lang： `ch`, `en`, `fr`, `german`, `korean`, `japan`
 
   默认为ch，中文，如果要修改识别语言；
 
   ```python
-  ocr(lang="ch") 
+  OCR.ocr(lang="ch") 
   ```
 
 - 匹配度
 
   similarity: float
 
   默认为0.6，可以修改为从0到1的数；
 
   ```shell
-  ocr(similarity=0.1)
+  OCR.ocr(similarity=0.1)
   ```
 
 - 返回原始数据
 
   return_default: bool
 
   默认为False，即默认返回识别到字符串的中心坐标，True表示返回原始数据；
 
   ```python
-  ocr(return_default=False)
+  OCR.ocr(return_default=False)
   ```
 
 - 只返回第一个
 
   return_first: bool
 
   当传入要查找的字符串时，可能存在当前屏幕中有多个目标；
 
   默认情况下是会将识别到的多个目标组装成字典返回；
 
   return_first=True 表示返回识别到的第一个。
 
   ```python
-  ocr(return_first=True )
+  OCR.ocr(return_first=True )
   ```
```

