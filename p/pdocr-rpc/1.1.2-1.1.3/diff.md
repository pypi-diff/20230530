# Comparing `tmp/pdocr_rpc-1.1.2.tar.gz` & `tmp/pdocr_rpc-1.1.3.tar.gz`

## Comparing `pdocr_rpc-1.1.2.tar` & `pdocr_rpc-1.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.2/pdocr_rpc/__init__.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.2/pdocr_rpc/__version__.py
--rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.2/pdocr_rpc/ocr.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.2/pdocr_rpc/ocr_server.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.2/pdocr_rpc/setting.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.2/LICENSE
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.2/README.md
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/pdocr_rpc/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/pdocr_rpc/__version__.py
+-rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/pdocr_rpc/ocr.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/pdocr_rpc/ocr_server.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/pdocr_rpc/setting.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 pdocr_rpc-1.1.3/PKG-INFO
```

### Comparing `pdocr_rpc-1.1.2/pdocr_rpc/ocr.py` & `pdocr_rpc-1.1.3/pdocr_rpc/ocr.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-1.1.2/pdocr_rpc/ocr_server.py` & `pdocr_rpc-1.1.3/pdocr_rpc/ocr_server.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-1.1.2/pdocr_rpc/setting.py` & `pdocr_rpc-1.1.3/pdocr_rpc/setting.py`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-1.1.2/LICENSE` & `pdocr_rpc-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdocr_rpc-1.1.2/README.md` & `pdocr_rpc-1.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,23 +22,23 @@
 
   ```shell
   pip3 install pillow
   ```
 
 - `Linux` 上安装截图工具：
 
-```shell
+```console
 pip3 install pyscreenshot
 ```
 
 ### 1.2、服务端依赖
 
 安装 `PaddleOCR` 环境：
 
-```shell
+```console
 pip3 install paddlepaddle -i https://mirror.baidu.com/pypi/simple
 pip3 install "paddleocr>=2.0.1" -i https://mirror.baidu.com/pypi/simple
 ```
 
 ## 2、使用方法
 
 ### 2.1、服务端
```

### Comparing `pdocr_rpc-1.1.2/pyproject.toml` & `pdocr_rpc-1.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pdocr-rpc"
-#version = "1.1.2"
 authors = [
   { name="mikigo", email="1964191531@qq.com" },
 ]
 description = "PaddleOCR-RPC"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -30,8 +29,7 @@
     "/pdocr_rpc",
     "/README.md",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/funny-test/pdocr-rpc"
 "Bug Tracker" = "https://github.com/funny-test/pdocr-rpc/issues"
-
```

### Comparing `pdocr_rpc-1.1.2/PKG-INFO` & `pdocr_rpc-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdocr-rpc
-Version: 1.1.2
+Version: 1.1.3
 Summary: PaddleOCR-RPC
 Project-URL: Homepage, https://github.com/funny-test/pdocr-rpc
 Project-URL: Bug Tracker, https://github.com/funny-test/pdocr-rpc/issues
 Author-email: mikigo <1964191531@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -37,23 +37,23 @@
 
   ```shell
   pip3 install pillow
   ```
 
 - `Linux` 上安装截图工具：
 
-```shell
+```console
 pip3 install pyscreenshot
 ```
 
 ### 1.2、服务端依赖
 
 安装 `PaddleOCR` 环境：
 
-```shell
+```console
 pip3 install paddlepaddle -i https://mirror.baidu.com/pypi/simple
 pip3 install "paddleocr>=2.0.1" -i https://mirror.baidu.com/pypi/simple
 ```
 
 ## 2、使用方法
 
 ### 2.1、服务端
```

