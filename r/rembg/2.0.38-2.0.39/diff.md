# Comparing `tmp/rembg-2.0.38.tar.gz` & `tmp/rembg-2.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rembg-2.0.38.tar", last modified: Mon May 29 17:08:31 2023, max compression
+gzip compressed data, was "rembg-2.0.39.tar", last modified: Tue May 30 04:51:08 2023, max compression
```

## Comparing `rembg-2.0.38.tar` & `rembg-2.0.39.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:08:31.911709 rembg-2.0.38/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-29 17:08:15.000000 rembg-2.0.38/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-29 17:08:15.000000 rembg-2.0.38/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13388 2023-05-29 17:08:31.911709 rembg-2.0.38/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12368 2023-05-29 17:08:15.000000 rembg-2.0.38/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-29 17:08:15.000000 rembg-2.0.38/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:08:31.911709 rembg-2.0.38/rembg/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-29 17:08:31.911709 rembg-2.0.38/rembg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/bg.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:08:31.907709 rembg-2.0.38/rembg/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/commands/b_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/commands/i_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/commands/p_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/commands/s_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/session_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:08:31.911709 rembg-2.0.38/rembg/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/sessions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/sessions/dis_anime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/sessions/dis_general_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/sessions/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/sessions/silueta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/sessions/u2net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/sessions/u2net_cloth_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/sessions/u2net_human_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-29 17:08:15.000000 rembg-2.0.38/rembg/sessions/u2netp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:08:31.903709 rembg-2.0.38/rembg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13388 2023-05-29 17:08:31.000000 rembg-2.0.38/rembg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-29 17:08:31.000000 rembg-2.0.38/rembg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:08:31.000000 rembg-2.0.38/rembg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 17:08:31.000000 rembg-2.0.38/rembg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-29 17:08:31.000000 rembg-2.0.38/rembg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 17:08:31.000000 rembg-2.0.38/rembg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 17:08:15.000000 rembg-2.0.38/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-29 17:08:15.000000 rembg-2.0.38/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-29 17:08:31.911709 rembg-2.0.38/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-29 17:08:15.000000 rembg-2.0.38/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-29 17:08:15.000000 rembg-2.0.38/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:51:08.814818 rembg-2.0.39/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-30 04:50:54.000000 rembg-2.0.39/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-30 04:50:54.000000 rembg-2.0.39/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-05-30 04:51:08.814818 rembg-2.0.39/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-05-30 04:50:54.000000 rembg-2.0.39/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-30 04:50:54.000000 rembg-2.0.39/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:51:08.814818 rembg-2.0.39/rembg/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-30 04:51:08.814818 rembg-2.0.39/rembg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/bg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:51:08.810818 rembg-2.0.39/rembg/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/commands/b_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/commands/i_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/commands/p_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/commands/s_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/session_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:51:08.814818 rembg-2.0.39/rembg/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/dis_anime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/dis_general_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/silueta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/u2net_cloth_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/u2net_human_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-30 04:50:54.000000 rembg-2.0.39/rembg/sessions/u2netp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 04:51:08.810818 rembg-2.0.39/rembg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-05-30 04:51:08.000000 rembg-2.0.39/rembg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-30 04:51:08.000000 rembg-2.0.39/rembg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 04:51:08.000000 rembg-2.0.39/rembg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 04:51:08.000000 rembg-2.0.39/rembg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-30 04:51:08.000000 rembg-2.0.39/rembg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 04:51:08.000000 rembg-2.0.39/rembg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-30 04:50:54.000000 rembg-2.0.39/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-30 04:50:54.000000 rembg-2.0.39/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-30 04:51:08.814818 rembg-2.0.39/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-30 04:50:54.000000 rembg-2.0.39/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-30 04:50:54.000000 rembg-2.0.39/versioneer.py
```

### Comparing `rembg-2.0.38/LICENSE.txt` & `rembg-2.0.39/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/PKG-INFO` & `rembg-2.0.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.38
+Version: 2.0.39
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 License: UNKNOWN
 Keywords: remove,background,u2net
 Platform: UNKNOWN
@@ -205,26 +205,26 @@
 rembg p -w path/to/input path/to/output
 ```
 
 ### rembg `s`
 
 Used to start http server.
 
-To see the complete endpoints documentation, go to: `http://localhost:5000/docs`.
+To see the complete endpoints documentation, go to: `http://localhost:5000/api`.
 
 Remove the background from an image url
 
 ```
-curl -s "http://localhost:5000/?url=http://input.png" -o output.png
+curl -s "http://localhost:5000/api/remove?url=http://input.png" -o output.png
 ```
 
 Remove the background from an uploaded image
 
 ```
-curl -s -F file=@/path/to/input.jpg "http://localhost:5000"  -o output.png
+curl -s -F file=@/path/to/input.jpg "http://localhost:5000/api/remove"  -o output.png
 ```
 
 ### rembg `b`
 
 Process a sequence of RGB24 images from stdin. This is intended to be used with another program, such as FFMPEG, that outputs RGB24 pixel data to stdout, which is piped into the stdin of this program, although nothing prevents you from manually typing in images at stdin.
 
 ```
```

### Comparing `rembg-2.0.38/README.md` & `rembg-2.0.39/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -178,26 +178,26 @@
 rembg p -w path/to/input path/to/output
 ```
 
 ### rembg `s`
 
 Used to start http server.
 
-To see the complete endpoints documentation, go to: `http://localhost:5000/docs`.
+To see the complete endpoints documentation, go to: `http://localhost:5000/api`.
 
 Remove the background from an image url
 
 ```
-curl -s "http://localhost:5000/?url=http://input.png" -o output.png
+curl -s "http://localhost:5000/api/remove?url=http://input.png" -o output.png
 ```
 
 Remove the background from an uploaded image
 
 ```
-curl -s -F file=@/path/to/input.jpg "http://localhost:5000"  -o output.png
+curl -s -F file=@/path/to/input.jpg "http://localhost:5000/api/remove"  -o output.png
 ```
 
 ### rembg `b`
 
 Process a sequence of RGB24 images from stdin. This is intended to be used with another program, such as FFMPEG, that outputs RGB24 pixel data to stdout, which is piped into the stdin of this program, although nothing prevents you from manually typing in images at stdin.
 
 ```
```

#### html2text {}

```diff
@@ -62,80 +62,81 @@
 alpha matting ``` rembg i -a path/to/input.png path/to/output.png ``` Passing
 extras parameters ``` rembg i -m sam -x '{"input_labels": [1], "input_points":
 [[100,100]]}' path/to/input.png path/to/output.png ``` ### rembg `p` Used when
 input and output are folders. Remove the background from all images in a folder
 ``` rembg p path/to/input path/to/output ``` Same as before, but watching for
 new/changed files to process ``` rembg p -w path/to/input path/to/output ```
 ### rembg `s` Used to start http server. To see the complete endpoints
-documentation, go to: `http://localhost:5000/docs`. Remove the background from
-an image url ``` curl -s "http://localhost:5000/?url=http://input.png" -
-o output.png ``` Remove the background from an uploaded image ``` curl -s -
-F file=@/path/to/input.jpg "http://localhost:5000" -o output.png ``` ### rembg
-`b` Process a sequence of RGB24 images from stdin. This is intended to be used
-with another program, such as FFMPEG, that outputs RGB24 pixel data to stdout,
-which is piped into the stdin of this program, although nothing prevents you
-from manually typing in images at stdin. ``` rembg b image_width image_height -
-o output_specifier ``` Arguments: - image_width : width of input image(s) -
-image_height : height of input image(s) - output_specifier: printf-style
-specifier for output filenames, for example if `output-%03u.png`, then output
-files will be named `output-000.png`, `output-001.png`, `output-002.png`, etc.
-Output files will be saved in PNG format regardless of the extension specified.
-You can omit it to write results to stdout. Example usage with FFMPEG: ```
-ffmpeg -i input.mp4 -ss 10 -an -f rawvideo -pix_fmt rgb24 pipe:1 | rembg b 1280
-720 -o folder/output-%03u.png ``` The width and height values must match the
-dimension of output images from FFMPEG. Note for FFMPEG, the "`-an -f rawvideo
--pix_fmt rgb24 pipe:1`" part is required for the whole thing to work. ## Usage
-as a library Input and output as bytes ```python from rembg import remove
-input_path = 'input.png' output_path = 'output.png' with open(input_path, 'rb')
-as i: with open(output_path, 'wb') as o: input = i.read() output = remove
-(input) o.write(output) ``` Input and output as a PIL image ```python from
-rembg import remove from PIL import Image input_path = 'input.png' output_path
-= 'output.png' input = Image.open(input_path) output = remove(input)
-output.save(output_path) ``` Input and output as a numpy array ```python from
-rembg import remove import cv2 input_path = 'input.png' output_path =
-'output.png' input = cv2.imread(input_path) output = remove(input) cv2.imwrite
-(output_path, output) ``` How to iterate over files in a performatic way
-```python from pathlib import Path from rembg import remove, new_session
-session = new_session() for file in Path('path/to/folder').glob('*.png'):
-input_path = str(file) output_path = str(file.parent / (file.stem +
-".out.png")) with open(input_path, 'rb') as i: with open(output_path, 'wb') as
-o: input = i.read() output = remove(input, session=session) o.write(output) ```
-To see a full list of examples on how to use rembg, go to the [examples]
-(USAGE.md) page. ## Usage as a docker Just replace the `rembg` command for
-`docker run danielgatis/rembg`. Try this: ``` docker run danielgatis/rembg i
-path/to/input.png path/to/output.png ``` ## Models All models are downloaded
-and saved in the user home folder in the `.u2net` directory. The available
-models are: - u2net ([download](https://github.com/danielgatis/rembg/releases/
-download/v0.0.0/u2net.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A
-pre-trained model for general use cases. - u2netp ([download](https://
-github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx), [source]
-(https://github.com/xuebinqin/U-2-Net)): A lightweight version of u2net model.
-- u2net_human_seg ([download](https://github.com/danielgatis/rembg/releases/
-download/v0.0.0/u2net_human_seg.onnx), [source](https://github.com/xuebinqin/U-
-2-Net)): A pre-trained model for human segmentation. - u2net_cloth_seg (
-[download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/
-u2net_cloth_seg.onnx), [source](https://github.com/levindabhi/cloth-
-segmentation)): A pre-trained model for Cloths Parsing from human portrait.
-Here clothes are parsed into 3 category: Upper body, Lower body and Full body.
-- silueta ([download](https://github.com/danielgatis/rembg/releases/download/
-v0.0.0/silueta.onnx), [source](https://github.com/xuebinqin/U-2-Net/issues/
-295)): Same as u2net but the size is reduced to 43Mb. - isnet-general-use (
-[download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-
-general-use.onnx), [source](https://github.com/xuebinqin/DIS)): A new pre-
-trained model for general use cases. - isnet-anime ([download](https://
-github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-anime.onnx),
-[source](https://github.com/SkyTNT/anime-segmentation)): A high-accuracy
-segmentation for anime character. - sam ([download encoder](https://github.com/
-danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-quant.onnx), [download
-decoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-
-decoder-quant.onnx), [source](https://github.com/facebookresearch/segment-
-anything)): A pre-trained model for any use cases. ### How to train your own
-model If You need more fine tunned models try this: https://github.com/
-danielgatis/rembg/issues/193#issuecomment-1055534289 ## Some video tutorials -
-https://www.youtube.com/watch?v=3xqwpXjxyMQ - https://www.youtube.com/
-watch?v=dFKRGXdkGJU - https://www.youtube.com/watch?v=Ai-BS_T7yjE - https://
-www.youtube.com/watch?v=dFKRGXdkGJU - https://www.youtube.com/watch?v=D7W-
-C0urVcQ ## References - https://arxiv.org/pdf/2005.09007.pdf - https://
-github.com/NathanUA/U-2-Net - https://github.com/pymatting/pymatting ## Buy me
-a coffee Liked some of my work? Buy me a coffee (or more likely a beer) [Buy_Me
-A_Coffee] ## License Copyright (c) 2020-present [Daniel Gatis](https://
-github.com/danielgatis) Licensed under [MIT License](./LICENSE.txt)
+documentation, go to: `http://localhost:5000/api`. Remove the background from
+an image url ``` curl -s "http://localhost:5000/api/remove?url=http://
+input.png" -o output.png ``` Remove the background from an uploaded image ```
+curl -s -F file=@/path/to/input.jpg "http://localhost:5000/api/remove" -
+o output.png ``` ### rembg `b` Process a sequence of RGB24 images from stdin.
+This is intended to be used with another program, such as FFMPEG, that outputs
+RGB24 pixel data to stdout, which is piped into the stdin of this program,
+although nothing prevents you from manually typing in images at stdin. ```
+rembg b image_width image_height -o output_specifier ``` Arguments: -
+image_width : width of input image(s) - image_height : height of input image(s)
+- output_specifier: printf-style specifier for output filenames, for example if
+`output-%03u.png`, then output files will be named `output-000.png`, `output-
+001.png`, `output-002.png`, etc. Output files will be saved in PNG format
+regardless of the extension specified. You can omit it to write results to
+stdout. Example usage with FFMPEG: ``` ffmpeg -i input.mp4 -ss 10 -an -
+f rawvideo -pix_fmt rgb24 pipe:1 | rembg b 1280 720 -o folder/output-%03u.png
+``` The width and height values must match the dimension of output images from
+FFMPEG. Note for FFMPEG, the "`-an -f rawvideo -pix_fmt rgb24 pipe:1`" part is
+required for the whole thing to work. ## Usage as a library Input and output as
+bytes ```python from rembg import remove input_path = 'input.png' output_path =
+'output.png' with open(input_path, 'rb') as i: with open(output_path, 'wb') as
+o: input = i.read() output = remove(input) o.write(output) ``` Input and output
+as a PIL image ```python from rembg import remove from PIL import Image
+input_path = 'input.png' output_path = 'output.png' input = Image.open
+(input_path) output = remove(input) output.save(output_path) ``` Input and
+output as a numpy array ```python from rembg import remove import cv2
+input_path = 'input.png' output_path = 'output.png' input = cv2.imread
+(input_path) output = remove(input) cv2.imwrite(output_path, output) ``` How to
+iterate over files in a performatic way ```python from pathlib import Path from
+rembg import remove, new_session session = new_session() for file in Path
+('path/to/folder').glob('*.png'): input_path = str(file) output_path = str
+(file.parent / (file.stem + ".out.png")) with open(input_path, 'rb') as i: with
+open(output_path, 'wb') as o: input = i.read() output = remove(input,
+session=session) o.write(output) ``` To see a full list of examples on how to
+use rembg, go to the [examples](USAGE.md) page. ## Usage as a docker Just
+replace the `rembg` command for `docker run danielgatis/rembg`. Try this: ```
+docker run danielgatis/rembg i path/to/input.png path/to/output.png ``` ##
+Models All models are downloaded and saved in the user home folder in the
+`.u2net` directory. The available models are: - u2net ([download](https://
+github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source]
+(https://github.com/xuebinqin/U-2-Net)): A pre-trained model for general use
+cases. - u2netp ([download](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)):
+A lightweight version of u2net model. - u2net_human_seg ([download](https://
+github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx),
+[source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for human
+segmentation. - u2net_cloth_seg ([download](https://github.com/danielgatis/
+rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx), [source](https://
+github.com/levindabhi/cloth-segmentation)): A pre-trained model for Cloths
+Parsing from human portrait. Here clothes are parsed into 3 category: Upper
+body, Lower body and Full body. - silueta ([download](https://github.com/
+danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://
+github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is
+reduced to 43Mb. - isnet-general-use ([download](https://github.com/
+danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source]
+(https://github.com/xuebinqin/DIS)): A new pre-trained model for general use
+cases. - isnet-anime ([download](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/isnet-anime.onnx), [source](https://github.com/SkyTNT/anime-
+segmentation)): A high-accuracy segmentation for anime character. - sam (
+[download encoder](https://github.com/danielgatis/rembg/releases/download/
+v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://github.com/
+danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-quant.onnx), [source]
+(https://github.com/facebookresearch/segment-anything)): A pre-trained model
+for any use cases. ### How to train your own model If You need more fine tunned
+models try this: https://github.com/danielgatis/rembg/issues/193#issuecomment-
+1055534289 ## Some video tutorials - https://www.youtube.com/
+watch?v=3xqwpXjxyMQ - https://www.youtube.com/watch?v=dFKRGXdkGJU - https://
+www.youtube.com/watch?v=Ai-BS_T7yjE - https://www.youtube.com/
+watch?v=dFKRGXdkGJU - https://www.youtube.com/watch?v=D7W-C0urVcQ ## References
+- https://arxiv.org/pdf/2005.09007.pdf - https://github.com/NathanUA/U-2-Net -
+https://github.com/pymatting/pymatting ## Buy me a coffee Liked some of my
+work? Buy me a coffee (or more likely a beer) [Buy_Me_A_Coffee] ## License
+Copyright (c) 2020-present [Daniel Gatis](https://github.com/danielgatis)
+Licensed under [MIT License](./LICENSE.txt)
```

### Comparing `rembg-2.0.38/rembg/bg.py` & `rembg-2.0.39/rembg/bg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/rembg/commands/b_command.py` & `rembg-2.0.39/rembg/commands/b_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/rembg/commands/i_command.py` & `rembg-2.0.39/rembg/commands/i_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/rembg/commands/p_command.py` & `rembg-2.0.39/rembg/commands/p_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/rembg/commands/s_command.py` & `rembg-2.0.39/rembg/commands/s_command.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import json
+import os
+import webbrowser
 from typing import Optional, Tuple, cast
 
 import aiohttp
 import click
+import gradio as gr
 import uvicorn
 from asyncer import asyncify
 from fastapi import Depends, FastAPI, File, Form, Query
 from fastapi.middleware.cors import CORSMiddleware
 from starlette.responses import Response
 
 from .._version import get_versions
@@ -66,14 +69,15 @@
             "email": "danielgatis@gmail.com",
         },
         license_info={
             "name": "MIT License",
             "url": "https://github.com/danielgatis/rembg/blob/main/LICENSE.txt",
         },
         openapi_tags=tags_metadata,
+        docs_url="/api",
     )
 
     app.add_middleware(
         CORSMiddleware,
         allow_credentials=True,
         allow_origins=["*"],
         allow_methods=["*"],
@@ -186,29 +190,34 @@
                 alpha_matting=commons.a,
                 alpha_matting_foreground_threshold=commons.af,
                 alpha_matting_background_threshold=commons.ab,
                 alpha_matting_erode_size=commons.ae,
                 only_mask=commons.om,
                 post_process_mask=commons.ppm,
                 bgcolor=commons.bgc,
-                **kwargs
+                **kwargs,
             ),
             media_type="image/png",
         )
 
     @app.on_event("startup")
     def startup():
+        try:
+            webbrowser.open(f"http://localhost:{port}")
+        except Exception:
+            pass
+
         if threads is not None:
             from anyio import CapacityLimiter
             from anyio.lowlevel import RunVar
 
             RunVar("_default_thread_limiter").set(CapacityLimiter(threads))
 
     @app.get(
-        path="/",
+        path="/api/remove",
         tags=["Background Removal"],
         summary="Remove from URL",
         description="Removes the background from an image obtained by retrieving an URL.",
     )
     async def get_index(
         url: str = Query(
             default=..., description="URL of the image that has to be processed."
@@ -217,22 +226,60 @@
     ):
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as response:
                 file = await response.read()
                 return await asyncify(im_without_bg)(file, commons)
 
     @app.post(
-        path="/",
+        path="/api/remove",
         tags=["Background Removal"],
         summary="Remove from Stream",
         description="Removes the background from an image sent within the request itself.",
     )
     async def post_index(
         file: bytes = File(
             default=...,
             description="Image file (byte stream) that has to be processed.",
         ),
         commons: CommonQueryPostParams = Depends(),
     ):
         return await asyncify(im_without_bg)(file, commons)  # type: ignore
 
-    uvicorn.run(app, host="0.0.0.0", port=port, log_level=log_level)
+    def gr_app(app):
+        def inference(input_path, model):
+            output_path = "output.png"
+            with open(input_path, "rb") as i:
+                with open(output_path, "wb") as o:
+                    input = i.read()
+                    output = remove(input, session=new_session(model))
+                    o.write(output)
+            return os.path.join(output_path)
+
+        interface = gr.Interface(
+            inference,
+            [
+                gr.components.Image(type="filepath", label="Input"),
+                gr.components.Dropdown(
+                    [
+                        "u2net",
+                        "u2netp",
+                        "u2net_human_seg",
+                        "u2net_cloth_seg",
+                        "silueta",
+                        "isnet-general-use",
+                        "isnet-anime",
+                    ],
+                    value="u2net",
+                    label="Models",
+                ),
+            ],
+            gr.components.Image(type="filepath", label="Output"),
+        )
+
+        interface.queue(concurrency_count=3)
+        app = gr.mount_gradio_app(app, interface, path="/")
+        return app
+
+    print(f"To access the API documentation, go to http://localhost:{port}/api")
+    print(f"To access the UI, go to http://localhost:{port}")
+
+    uvicorn.run(gr_app(app), host="0.0.0.0", port=port, log_level=log_level)
```

### Comparing `rembg-2.0.38/rembg/session_factory.py` & `rembg-2.0.39/rembg/session_factory.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/rembg/sessions/__init__.py` & `rembg-2.0.39/rembg/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/rembg/sessions/base.py` & `rembg-2.0.39/rembg/sessions/base.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/rembg/sessions/dis_anime.py` & `rembg-2.0.39/rembg/sessions/dis_anime.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/rembg/sessions/dis_general_use.py` & `rembg-2.0.39/rembg/sessions/dis_general_use.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/rembg/sessions/sam.py` & `rembg-2.0.39/rembg/sessions/sam.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/rembg/sessions/silueta.py` & `rembg-2.0.39/rembg/sessions/silueta.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/rembg/sessions/u2net.py` & `rembg-2.0.39/rembg/sessions/u2net.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/rembg/sessions/u2net_cloth_seg.py` & `rembg-2.0.39/rembg/sessions/u2net_cloth_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/rembg/sessions/u2net_human_seg.py` & `rembg-2.0.39/rembg/sessions/u2net_human_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/rembg/sessions/u2netp.py` & `rembg-2.0.39/rembg/sessions/u2netp.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/rembg.egg-info/PKG-INFO` & `rembg-2.0.39/rembg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.38
+Version: 2.0.39
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 License: UNKNOWN
 Keywords: remove,background,u2net
 Platform: UNKNOWN
@@ -205,26 +205,26 @@
 rembg p -w path/to/input path/to/output
 ```
 
 ### rembg `s`
 
 Used to start http server.
 
-To see the complete endpoints documentation, go to: `http://localhost:5000/docs`.
+To see the complete endpoints documentation, go to: `http://localhost:5000/api`.
 
 Remove the background from an image url
 
 ```
-curl -s "http://localhost:5000/?url=http://input.png" -o output.png
+curl -s "http://localhost:5000/api/remove?url=http://input.png" -o output.png
 ```
 
 Remove the background from an uploaded image
 
 ```
-curl -s -F file=@/path/to/input.jpg "http://localhost:5000"  -o output.png
+curl -s -F file=@/path/to/input.jpg "http://localhost:5000/api/remove"  -o output.png
 ```
 
 ### rembg `b`
 
 Process a sequence of RGB24 images from stdin. This is intended to be used with another program, such as FFMPEG, that outputs RGB24 pixel data to stdout, which is piped into the stdin of this program, although nothing prevents you from manually typing in images at stdin.
 
 ```
```

### Comparing `rembg-2.0.38/rembg.egg-info/SOURCES.txt` & `rembg-2.0.39/rembg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.38/setup.py` & `rembg-2.0.39/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     python_requires=">3.7, <3.11",
     install_requires=[
         "aiohttp>=3.8.1",
         "asyncer>=0.0.2",
         "click>=8.1.3",
         "fastapi>=0.92.0",
         "filetype>=1.2.0",
+        "gradio>=3.32.0",
         "imagehash>=4.3.1",
         "numpy>=1.23.5",
         "onnxruntime>=1.14.1",
         "opencv-python-headless>=4.6.0.66",
         "pillow>=9.3.0",
         "pooch>=1.6.0",
         "pymatting>=1.1.8",
```

### Comparing `rembg-2.0.38/versioneer.py` & `rembg-2.0.39/versioneer.py`

 * *Files identical despite different names*

