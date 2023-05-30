# Comparing `tmp/pdocr-rpc-1.1.0.tar.gz` & `tmp/pdocr-rpc-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/uos/github/pdocr-rpc/dist/.tmp-vxzn6xlk/pdocr-rpc-1.1.0.tar", last modified: Tue May 30 02:19:53 2023, max compression
+gzip compressed data, was "/home/uos/github/pdocr-rpc/dist/.tmp-g4k48f5e/pdocr-rpc-1.1.1.tar", last modified: Tue May 30 03:32:16 2023, max compression
```

## Comparing `pdocr-rpc-1.1.0.tar` & `pdocr-rpc-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/
--rw-r--r--   0 uos       (1000) uos       (1000)    11357 2023-05-26 08:16:45.000000 pdocr-rpc-1.1.0/LICENSE
--rw-r--r--   0 uos       (1000) uos       (1000)     3200 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/PKG-INFO
--rw-r--r--   0 uos       (1000) uos       (1000)     2702 2023-05-30 02:15:13.000000 pdocr-rpc-1.1.0/README.md
-drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/pdocr_rpc/
--rw-r--r--   0 uos       (1000) uos       (1000)        0 2023-05-26 09:13:53.000000 pdocr-rpc-1.1.0/pdocr_rpc/__init__.py
--rw-r--r--   0 uos       (1000) uos       (1000)     5752 2023-05-26 10:18:48.000000 pdocr-rpc-1.1.0/pdocr_rpc/ocr.py
--rw-r--r--   0 uos       (1000) uos       (1000)     1474 2023-05-30 02:02:07.000000 pdocr-rpc-1.1.0/pdocr_rpc/ocr_server.py
--rw-r--r--   0 uos       (1000) uos       (1000)      904 2023-05-26 10:18:24.000000 pdocr-rpc-1.1.0/pdocr_rpc/setting.py
-drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/pdocr_rpc.egg-info/
--rw-r--r--   0 uos       (1000) uos       (1000)     3200 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/pdocr_rpc.egg-info/PKG-INFO
--rw-r--r--   0 uos       (1000) uos       (1000)      265 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/pdocr_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 uos       (1000) uos       (1000)        1 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/pdocr_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 uos       (1000) uos       (1000)       10 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/pdocr_rpc.egg-info/top_level.txt
--rw-r--r--   0 uos       (1000) uos       (1000)      482 2023-05-30 02:16:10.000000 pdocr-rpc-1.1.0/pyproject.toml
--rw-r--r--   0 uos       (1000) uos       (1000)       38 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/setup.cfg
-drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-30 02:19:53.000000 pdocr-rpc-1.1.0/test/
--rw-r--r--   0 uos       (1000) uos       (1000)      169 2023-05-30 02:02:07.000000 pdocr-rpc-1.1.0/test/test_ocr.py
+drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-30 03:32:16.000000 pdocr-rpc-1.1.1/
+-rw-r--r--   0 uos       (1000) uos       (1000)    11357 2023-05-26 08:16:45.000000 pdocr-rpc-1.1.1/LICENSE
+-rw-r--r--   0 uos       (1000) uos       (1000)     3197 2023-05-30 03:32:16.000000 pdocr-rpc-1.1.1/PKG-INFO
+-rw-r--r--   0 uos       (1000) uos       (1000)     2700 2023-05-30 02:26:10.000000 pdocr-rpc-1.1.1/README.md
+drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-30 03:32:16.000000 pdocr-rpc-1.1.1/pdocr_rpc/
+-rw-r--r--   0 uos       (1000) uos       (1000)        0 2023-05-26 09:13:53.000000 pdocr-rpc-1.1.1/pdocr_rpc/__init__.py
+-rw-r--r--   0 uos       (1000) uos       (1000)     5802 2023-05-30 03:28:52.000000 pdocr-rpc-1.1.1/pdocr_rpc/ocr.py
+-rw-r--r--   0 uos       (1000) uos       (1000)     1474 2023-05-30 03:28:52.000000 pdocr-rpc-1.1.1/pdocr_rpc/ocr_server.py
+-rw-r--r--   0 uos       (1000) uos       (1000)      942 2023-05-30 03:28:52.000000 pdocr-rpc-1.1.1/pdocr_rpc/setting.py
+drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-30 03:32:16.000000 pdocr-rpc-1.1.1/pdocr_rpc.egg-info/
+-rw-r--r--   0 uos       (1000) uos       (1000)     3197 2023-05-30 03:32:16.000000 pdocr-rpc-1.1.1/pdocr_rpc.egg-info/PKG-INFO
+-rw-r--r--   0 uos       (1000) uos       (1000)      265 2023-05-30 03:32:16.000000 pdocr-rpc-1.1.1/pdocr_rpc.egg-info/SOURCES.txt
+-rw-r--r--   0 uos       (1000) uos       (1000)        1 2023-05-30 03:32:16.000000 pdocr-rpc-1.1.1/pdocr_rpc.egg-info/dependency_links.txt
+-rw-r--r--   0 uos       (1000) uos       (1000)       10 2023-05-30 03:32:16.000000 pdocr-rpc-1.1.1/pdocr_rpc.egg-info/top_level.txt
+-rw-r--r--   0 uos       (1000) uos       (1000)      482 2023-05-30 03:32:06.000000 pdocr-rpc-1.1.1/pyproject.toml
+-rw-r--r--   0 uos       (1000) uos       (1000)       38 2023-05-30 03:32:16.000000 pdocr-rpc-1.1.1/setup.cfg
+drwxr-xr-x   0 uos       (1000) uos       (1000)        0 2023-05-30 03:32:16.000000 pdocr-rpc-1.1.1/test/
+-rw-r--r--   0 uos       (1000) uos       (1000)      264 2023-05-30 03:29:16.000000 pdocr-rpc-1.1.1/test/test_ocr.py
```

### Comparing `pdocr-rpc-1.1.0/LICENSE` & `pdocr-rpc-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdocr-rpc-1.1.0/PKG-INFO` & `pdocr-rpc-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdocr-rpc
-Version: 1.1.0
+Version: 1.1.1
 Summary: PaddleOCR-RPC
 Author-email: mikigo <1964191531@qq.com>
 Project-URL: Homepage, https://github.com/funny-test/pdocr-rpc
 Project-URL: Bug Tracker, https://github.com/funny-test/pdocr-rpc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 
 # pdocr-rpc
 
 基于 `PaddleOCR` 封装的 `RPC` 服务，包含客户端和服务端。
 
 客户端提供了一个简单易用的函数 `ocr`，通过不同的参数控制返回不同的值。
 
-Document：https://funny-test.github.io/pdocr-rpc
+Documents：https://funny-test.github.io/pdocr-rpc
 
 ## 1、安装
 
 ```shell
 pip install pdocr-rpc
 ```
 
@@ -36,17 +36,17 @@
 
   ```shell
   pip3 install pillow
   ```
 
 - `Linux` 上安装截图工具：
 
-  ```shell
+```shell
 pip3 install pyscreenshot
-  ```
+```
 
 ### 1.2、服务端依赖
 
 安装 `PaddleOCR` 环境：
 
 ```shell
 pip3 install paddlepaddle -i https://mirror.baidu.com/pypi/simple
```

### Comparing `pdocr-rpc-1.1.0/README.md` & `pdocr-rpc-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pdocr-rpc
 
 基于 `PaddleOCR` 封装的 `RPC` 服务，包含客户端和服务端。
 
 客户端提供了一个简单易用的函数 `ocr`，通过不同的参数控制返回不同的值。
 
-Document：https://funny-test.github.io/pdocr-rpc
+Documents：https://funny-test.github.io/pdocr-rpc
 
 ## 1、安装
 
 ```shell
 pip install pdocr-rpc
 ```
 
@@ -22,17 +22,17 @@
 
   ```shell
   pip3 install pillow
   ```
 
 - `Linux` 上安装截图工具：
 
-  ```shell
+```shell
 pip3 install pyscreenshot
-  ```
+```
 
 ### 1.2、服务端依赖
 
 安装 `PaddleOCR` 环境：
 
 ```shell
 pip3 install paddlepaddle -i https://mirror.baidu.com/pypi/simple
@@ -143,8 +143,8 @@
 
   return_first=True 表示返回识别到的第一个。
 
   ```python
   ocr(return_first=True )
   ```
 
-  
+
```

### Comparing `pdocr-rpc-1.1.0/pdocr_rpc/ocr.py` & `pdocr-rpc-1.1.1/pdocr_rpc/ocr.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,55 +16,65 @@
 
 if setting.IS_LINUX:
     import pyscreenshot as ImageGrab
 elif setting.IS_WINDOWS:
     from PIL import ImageGrab
 
 
-def _pdocr_client(lang, picture_abspath=None):
+def _pdocr_client(lang, picture_abspath=None, retry: int = 2):
     """
      通过 RPC 协议进行 OCR 识别。
     :return: 返回 PaddleOCR 的原始数据
     """
     if not picture_abspath:
         picture_abspath = setting.SCREEN_CACHE
         if setting.IS_X11:
             ImageGrab.grab().save(os.path.expanduser(picture_abspath))
         else:
             picture_abspath = (
                 popen("qdbus org.kde.KWin /Screenshot screenshotFullscreen")
-                    .read()
-                    .strip("\n")
+                .read()
+                .strip("\n")
             )
     server = ServerProxy(f"http://{setting.SERVER_IP}:{setting.PORT}", allow_none=True)
     put_handle = open(os.path.expanduser(picture_abspath), "rb")
-    try:
-        # 将图片上传到服务端
-        pic_dir = server.image_put(Binary(put_handle.read()))
-        put_handle.close()
-        # 返回识别结果
-        return server.paddle_ocr(pic_dir, lang)
-    except OSError:
+    for _ in range(retry):
+        try:
+            # 将图片上传到服务端
+            pic_dir = server.image_put(Binary(put_handle.read()))
+            put_handle.close()
+            # 返回识别结果
+            return server.paddle_ocr(pic_dir, lang)
+        except OSError:
+            pass
         raise EnvironmentError(f"RPC服务器链接失败. http://{setting.SERVER_IP}:{setting.PORT}")
 
 
-def ocr(*target_strings, picture_abspath=None, similarity=0.6, return_default=False, return_first=False, lang="ch"):
+def ocr(
+    *target_strings,
+    picture_abspath=None,
+    similarity=0.6,
+    return_default=False,
+    return_first=False,
+    lang="ch",
+    retry: int = 2,
+):
     """
      通过 OCR 进行识别。
     :param target_strings:
         目标字符,识别一个字符串或多个字符串,并返回其在图片中的坐标;
         如果不传参，返回图片中识别到的所有字符串。
     :param picture_abspath: 要识别的图片路径，如果不传默认截取全屏识别。
     :param similarity: 匹配度。
     :param return_default: 返回识别的原生数据。
     :param return_first: 只返回第一个,默认为 False,返回识别到的所有数据。
     :param lang: `ch`, `en`, `fr`, `german`, `korean`, `japan`
     :return: 返回的坐标是目标字符串所在行的中心坐标。
     """
-    results = _pdocr_client(picture_abspath=picture_abspath, lang=lang)
+    results = _pdocr_client(picture_abspath=picture_abspath, lang=lang, retry=retry)
     if return_default:
         return results
     more_map = {}
     if len(target_strings) == 1:
         n = 1
         for res in results:
             [
@@ -89,17 +99,15 @@
                         break
                     n += 1
         if len(more_map) == 1:
             center_x, center_y = more_map.get(target_strings[0])
             print(f"OCR识别到字符“{target_strings[0]}”—>{center_x, center_y}")
             return center_x, center_y
         if len(more_map) > 1:
-            print(
-                f"OCR识别结果:\n{json.dumps(more_map, ensure_ascii=False, indent=2)}"
-            )
+            print(f"OCR识别结果:\n{json.dumps(more_map, ensure_ascii=False, indent=2)}")
             return more_map
 
     elif len(target_strings) == 0:
         for res in results:
             [
                 [
                     [left_top_x, left_top_y],
@@ -111,17 +119,15 @@
             ] = res
             if rate >= similarity:
                 center_x = (right_top_x + left_top_x) / 2
                 center_y = (right_bottom_y + right_top_y) / 2
                 more_map[strings] = (center_x, center_y)
 
         if more_map:
-            print(
-                f"OCR识别结果:\n{json.dumps(more_map, ensure_ascii=False, indent=2)}"
-            )
+            print(f"OCR识别结果:\n{json.dumps(more_map, ensure_ascii=False, indent=2)}")
             return more_map
 
     else:
         for target_string in target_strings:
             n = 1
             more_map[target_string] = False
             for res in results:
@@ -144,18 +150,16 @@
                         n = 1
                     more_map[_key] = (center_x, center_y)
                     if return_first:
                         break
                     n += 1
 
         if more_map:
-            print(
-                f"OCR识别结果:\n{json.dumps(more_map, ensure_ascii=False, indent=2)}"
-            )
+            print(f"OCR识别结果:\n{json.dumps(more_map, ensure_ascii=False, indent=2)}")
             return more_map
 
     print(f"未识别到字符{f'“{target_strings}”' or ''}")
     return False
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     print(ocr())
```

### Comparing `pdocr-rpc-1.1.0/pdocr_rpc/ocr_server.py` & `pdocr-rpc-1.1.1/pdocr_rpc/ocr_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 def image_put(data):
     pic_dir = join(CURRENT_DIR, "pic")
     if not exists(pic_dir):
         makedirs(pic_dir)
 
-    pic_path = join(pic_dir, f'pic_{time()}.png')
+    pic_path = join(pic_dir, f"pic_{time()}.png")
     handle = open(pic_path, "wb")
     handle.write(data.data)
     handle.close()
     return pic_path
 
 
 def paddle_ocr(pic_path, lang):
```

### Comparing `pdocr-rpc-1.1.0/pdocr_rpc/setting.py` & `pdocr-rpc-1.1.1/pdocr_rpc/setting.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import enum
 import os
 import sys
 
+
 @enum.unique
 class DisplayServer(enum.Enum):
     wayland = "wayland"
     x11 = "x11"
 
+
 @enum.unique
 class PlatForm(enum.Enum):
     win = "win32"
     linux = "linux"
 
 
-
 class _Setting:
     """配置模块"""
 
     SERVER_IP = "127.0.0.1"
     PORT = 8890
 
     IS_LINUX = False
@@ -27,17 +28,20 @@
         IS_WINDOWS = True
         # TODO
         ...
     elif sys.platform == PlatForm.linux.value:
         # Linux
         IS_LINUX = True
         # 显示服务器
-        DISPLAY_SERVER = os.popen(
-            "cat ~/.xsession-errors | grep XDG_SESSION_TYPE | head -n 1"
-        ).read().split("=")[-1].strip("\n")
+        DISPLAY_SERVER = (
+            os.popen("cat ~/.xsession-errors | grep XDG_SESSION_TYPE | head -n 1")
+            .read()
+            .split("=")[-1]
+            .strip("\n")
+        )
 
-        IS_X11 = (DISPLAY_SERVER == DisplayServer.x11.value)
-        IS_WAYLAND = (DISPLAY_SERVER == DisplayServer.wayland.value)
+        IS_X11 = DISPLAY_SERVER == DisplayServer.x11.value
+        IS_WAYLAND = DISPLAY_SERVER == DisplayServer.wayland.value
         SCREEN_CACHE = "/tmp/screen.png"
 
 
 setting = _Setting()
```

### Comparing `pdocr-rpc-1.1.0/pdocr_rpc.egg-info/PKG-INFO` & `pdocr-rpc-1.1.1/pdocr_rpc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdocr-rpc
-Version: 1.1.0
+Version: 1.1.1
 Summary: PaddleOCR-RPC
 Author-email: mikigo <1964191531@qq.com>
 Project-URL: Homepage, https://github.com/funny-test/pdocr-rpc
 Project-URL: Bug Tracker, https://github.com/funny-test/pdocr-rpc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 
 # pdocr-rpc
 
 基于 `PaddleOCR` 封装的 `RPC` 服务，包含客户端和服务端。
 
 客户端提供了一个简单易用的函数 `ocr`，通过不同的参数控制返回不同的值。
 
-Document：https://funny-test.github.io/pdocr-rpc
+Documents：https://funny-test.github.io/pdocr-rpc
 
 ## 1、安装
 
 ```shell
 pip install pdocr-rpc
 ```
 
@@ -36,17 +36,17 @@
 
   ```shell
   pip3 install pillow
   ```
 
 - `Linux` 上安装截图工具：
 
-  ```shell
+```shell
 pip3 install pyscreenshot
-  ```
+```
 
 ### 1.2、服务端依赖
 
 安装 `PaddleOCR` 环境：
 
 ```shell
 pip3 install paddlepaddle -i https://mirror.baidu.com/pypi/simple
```

