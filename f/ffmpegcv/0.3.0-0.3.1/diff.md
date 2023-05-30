# Comparing `tmp/ffmpegcv-0.3.0.tar.gz` & `tmp/ffmpegcv-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpegcv-0.3.0.tar", last modified: Wed May 10 17:08:58 2023, max compression
+gzip compressed data, was "dist/ffmpegcv-0.3.1.tar", last modified: Tue May 30 19:22:10 2023, max compression
```

## Comparing `ffmpegcv-0.3.0.tar` & `ffmpegcv-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-05-10 17:08:58.114086 ffmpegcv-0.3.0/
--rw-r--r--   0 chen       (501) staff       (20)    11532 2023-05-10 17:08:58.113894 ffmpegcv-0.3.0/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)     9166 2023-05-10 17:04:34.000000 ffmpegcv-0.3.0/README.md
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-05-10 17:08:58.112961 ffmpegcv-0.3.0/ffmpegcv/
--rw-r--r--   0 chen       (501) staff       (20)     7729 2023-05-09 14:16:12.000000 ffmpegcv-0.3.0/ffmpegcv/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     9202 2023-05-09 14:16:12.000000 ffmpegcv-0.3.0/ffmpegcv/ffmpeg_reader.py
--rw-r--r--   0 chen       (501) staff       (20)    14598 2023-05-10 17:05:37.000000 ffmpegcv-0.3.0/ffmpegcv/ffmpeg_reader_camera.py
--rw-r--r--   0 chen       (501) staff       (20)     3731 2023-05-09 14:16:12.000000 ffmpegcv-0.3.0/ffmpegcv/ffmpeg_writer.py
--rw-r--r--   0 chen       (501) staff       (20)     2878 2023-05-09 14:16:12.000000 ffmpegcv-0.3.0/ffmpegcv/video_info.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-05-10 17:08:58.113579 ffmpegcv-0.3.0/ffmpegcv.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)    11532 2023-05-10 17:08:58.000000 ffmpegcv-0.3.0/ffmpegcv.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      275 2023-05-10 17:08:58.000000 ffmpegcv-0.3.0/ffmpegcv.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2023-05-10 17:08:58.000000 ffmpegcv-0.3.0/ffmpegcv.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)        9 2023-05-10 17:08:58.000000 ffmpegcv-0.3.0/ffmpegcv.egg-info/top_level.txt
--rw-r--r--   0 chen       (501) staff       (20)       38 2023-05-10 17:08:58.114137 ffmpegcv-0.3.0/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      544 2023-05-10 17:08:45.000000 ffmpegcv-0.3.0/setup.py
+drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10392 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/PKG-INFO
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10179 2023-05-30 19:12:16.000000 ffmpegcv-0.3.1/README.md
+drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/ffmpegcv/
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10453 2023-05-30 19:18:41.000000 ffmpegcv-0.3.1/ffmpegcv/__init__.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     5265 2022-05-18 13:48:31.000000 ffmpegcv-0.3.1/ffmpegcv/ffmpeg_framepick.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     9732 2023-05-30 14:58:25.000000 ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    15029 2023-05-30 14:58:25.000000 ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader_camera.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1685 2022-05-19 12:21:02.000000 ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader_grey.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1474 2022-06-04 11:24:12.000000 ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader_hflip.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2618 2022-05-19 17:30:20.000000 ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader_laggy.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3935 2023-05-30 19:00:58.000000 ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader_stream.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3989 2023-05-30 15:02:00.000000 ffmpegcv-0.3.1/ffmpegcv/ffmpeg_writer.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1053 2023-05-30 17:50:58.000000 ffmpegcv-0.3.1/ffmpegcv/stream_info.py
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2731 2023-05-30 15:03:32.000000 ffmpegcv-0.3.1/ffmpegcv/video_info.py
+drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/ffmpegcv.egg-info/
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)    10392 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/ffmpegcv.egg-info/PKG-INFO
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      487 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/ffmpegcv.egg-info/SOURCES.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        1 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/ffmpegcv.egg-info/dependency_links.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        6 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/ffmpegcv.egg-info/requires.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        9 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/ffmpegcv.egg-info/top_level.txt
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)       38 2023-05-30 19:22:10.000000 ffmpegcv-0.3.1/setup.cfg
+-rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      643 2023-05-30 19:21:17.000000 ffmpegcv-0.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ffmpegcv-0.3.0/PKG-INFO` & `ffmpegcv-0.3.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,275 +1,299 @@
-Metadata-Version: 2.1
-Name: ffmpegcv
-Version: 0.3.0
-Summary: UNKNOWN
-Home-page: https://pypi.org/project/ffmpegcv/
-Author: chenxf
-Author-email: cxf529125853@163.com
-License: UNKNOWN
-Description: # FFMPEGCV is an alternative to OPENCV for video read and write.
-        The ffmpegcv provide Video Reader and Video Witer with ffmpeg backbone, which are faster and powerful than cv2.
-        
-        - The ffmpegcv is api **compatible** to open-cv. 
-        - The ffmpegcv can use **GPU accelerate** encoding and decoding*. 
-        - The ffmpegcv support much more video **codecs** v.s. open-cv.
-        - The ffmpegcv support **RGB** & BGR format as you like.
-        - The ffmpegcv can support ROI operations.You can **crop**, **resize** and **pad** the ROI.
-        
-        In all, ffmpegcv is just similar to opencv api. But is faster* and with more codecs.
-        
-        
-        ## Basic example
-        Read a video by CPU, and rewrite it by GPU.
-        ```python
-        vidin = ffmpegcv.VideoCapture(vfile_in)
-        vidout = ffmpegcv.VideoWriterNV(vfile_out, 'h264', vidin.fps)
-        
-        with vidin, vidout:
-            for frame in vidin:
-                cv2.imshow('image', frame)
-                vidout.write(frame)
-        ```
-        
-        Read the camera by device name.
-        ```python
-        cap = ffmpegcv.VideoCaptureCAM("Integrated Camera")
-        ```
-        
-        ## Install
-        You need to download ffmpeg before you can use ffmpegcv
-        > conda install ffmpeg 
-        >
-        > pip install ffmpegcv
-        
-        ## GPU Accelation
-        - Support NVIDIA card only.
-        - Perfect in the **Windows**. That ffmpeg supports NVIDIA acceleration just by conda install.
-        - Struggle in the **Linux**. That ffmpeg didn't orginally support NVIDIA accelerate.
-        Please re-compile the ffmpeg by yourself.
-        See the [link](https://docs.nvidia.com/video-technologies/video-codec-sdk/ffmpeg-with-nvidia-gpu/)
-        - Works in the **Google Colab** notebook without pain (no need to recompile ffmpeg). 
-        - Infeasible in the **MacOS**. That ffmpeg didn't supports NVIDIA at all.
-        
-        > \* The ffmegcv GPU reader is a bit slower than CPU reader, but much faster when use ROI operations (crop, resize, pad).
-        
-        ## Codecs
-        
-        | Codecs      | OpenCV-reader | ffmpegcv-cpu-r     | gpu-r  | OpenCV-writer | ffmpegcv-cpu-w     | gpu-w  |
-        | ----------- | ------------- | ---------------- | ---- | ------------- | ---------------- | ---- |
-        | h264        | √             | √                | √    | ×             | √                | √    |
-        | h265 (hevc) | not sure      | √                | √    | ×             | √                | √    |
-        | mjpeg       | √             | √                | ×    | √             | √                | ×    |
-        | mpeg        | √             | √                | ×    | √             | √                | ×    |
-        | others      | not sure      | ffmpeg -decoders | ×    | not sure      | ffmpeg -encoders | ×    |
-        
-        ## Benchmark
-        *On the way...*
-        
-        
-        ## Video Reader
-        ---
-        The ffmpegcv is just similar to opencv in api.
-        ```python
-        # open cv
-        import cv2
-        cap = cv2.VideoCapture(file)
-        while True:
-            ret, frame = cap.read()
-            if not ret:
-                break
-            pass
-        
-        # ffmpegcv
-        import ffmpegcv
-        cap = ffmpegcv.VideoCapture(file)
-        while True:
-            ret, frame = cap.read()
-            if not ret:
-                break
-            pass
-        cap.release()
-        
-        # alternative
-        cap = ffmpegcv.VideoCapture(file)
-        nframe = len(cap)
-        for frame in cap:
-            pass
-        cap.release()
-        
-        # more pythonic, recommand
-        with ffmpegcv.VideoCapture(file) as cap:
-            nframe = len(cap)
-            for iframe, frame in enumerate(cap):
-                if iframe>100: break
-                pass
-        ```
-        
-        Use GPU to accelerate decoding. It depends on the video codes.
-        h264_nvcuvid, hevc_nvcuvid ....
-        ```python
-        cap_cpu = ffmpegcv.VideoCapture(file)
-        cap_gpu = ffmpegcv.VideoCapture(file, codec='h264_cuvid') #NVIDIA GPU0
-        cap_gpu0 = ffmpegcv.VideoCaptureNV(file)         #NVIDIA GPU0
-        cap_gpu1 = ffmpegcv.VideoCaptureNV(file, gpu=1)  #NVIDIA GPU1
-        ```
-        
-        Use rgb24 instead of bgr24
-        ```python
-        cap = ffmpegcv.VideoCapture(file, pix_fmt='rgb24')
-        ret, frame = cap.read()
-        plt.imshow(frame)
-        ```
-        
-        ### ROI Operations
-        You can crop, resize and pad the video. These ROI operation is `ffmpegcv-GPU` > `ffmpegcv-CPU` >> `opencv`.
-        
-        **Crop** video, which will be much faster than read the whole canvas.
-        ```python
-        cap = ffmpegcv.VideoCapture(file, crop_xywh=(0, 0, 640, 480))
-        ```
-        
-        **Resize** the video to the given size.
-        ```python
-        cap = ffmpegcv.VideoCapture(file, resize=(640, 480))
-        ```
-        
-        **Resize** and keep the aspect ratio with black border **padding**.
-        ```python
-        cap = ffmpegcv.VideoCapture(file, resize=(640, 480), resize_keepratio=True)
-        ```
-        
-        **Crop** and then **resize** the video.
-        ```python
-        cap = ffmpegcv.VideoCapture(file, crop_xywh=(0, 0, 640, 480), resize=(512, 512))
-        ```
-        
-        ## Video Writer
-        ---
-        ```python
-        # cv2
-        out = cv2.VideoWriter('outpy.avi',
-                               cv2.VideoWriter_fourcc('M','J','P','G'), 
-                               10, 
-                               (w, h))
-        out.write(frame1)
-        out.write(frame2)
-        out.release()
-        
-        # ffmpegcv, default codec is 'h264' in cpu 'h265' in gpu.
-        # frameSize is decided by the size of the first frame
-        out = ffmpegcv.VideoWriter('outpy.mp4', None, 10)
-        out.write(frame1)
-        out.write(frame2)
-        out.release()
-        
-        # more pythonic
-        with ffmpegcv.VideoWriter('outpy.mp4', None, 10) as out:
-            out.write(frame1)
-            out.write(frame2)
-        ```
-        
-        
-        Use GPU to accelerate encoding. Such as h264_nvenc, hevc_nvenc.
-        ```python
-        out_cpu = ffmpegcv.VideoWriter('outpy.mp4', None, 10)
-        out_gpu0 = ffmpegcv.VideoWriterNV('outpy.mp4', 'h264', 10)        #NVIDIA GPU0
-        out_gpu1 = ffmpegcv.VideoWriterNV('outpy.mp4', 'hevc', 10, gpu=1) #NVIDIA GPU1
-        ```
-        
-        Input image is rgb24 instead of bgr24
-        ```python
-        out = ffmpegcv.VideoWriter('outpy.mp4', None, 10, pix_fmt='rgb24')
-        out.write(cv2.cvtColor(frame, cv2.COLOR_BGR2RGB))
-        ```
-        
-        ## Video Reader and Writer
-        ---
-        ```python
-        import ffmpegcv
-        vfile_in = 'A.mp4'
-        vfile_out = 'A_h264.mp4'
-        vidin = ffmpegcv.VideoCapture(vfile_in)
-        vidout = ffmpegcv.VideoWriter(vfile_out, None, vidin.fps)
-        
-        with vidin, vidout:
-            for frame in vidin:
-                vidout.write(frame)
-        ```
-        
-        ## Camera Reader
-        ---
-        ***Experimental feature**. The ffmpegcv offers Camera reader. Which is consistent with VideoFiler reader. 
-        
-        - The `VideoCaptureCAM` aims to support ROI operations. The Opencv will be general fascinating than ffmpegcv in camera read. **I recommand the opencv in most camera reading case**.
-        - The ffmpegcv can use name to retrieve the camera device. Use `ffmpegcv.VideoCaptureCAM("Integrated Camera")` is readable than `cv2.VideoCaptureCAM(0)`.
-        - The `VideoCaptureCAM` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
-        - The `VideoCaptureCAM` is continously working on background even if you didn't read it. Please release it in time.
-        - Works perfect in Windows, not-perfect in Linux and macOS.
-        
-        ```python
-        import cv2
-        cap = cv2.VideoCapture(0)
-        while True:
-            ret, frame = cap.read()
-            cv2.imshow('frame', frame)
-            if cv2.waitKey(1) & 0xFF == ord('q'):
-                break
-        cap.release()
-        
-        # ffmpegcv, in Windows&Linux
-        import ffmpegcv
-        cap = ffmpegcv.VideoCaptureCAM(0)
-        while True:
-            ret, frame = cap.read()
-            cv2.imshow('frame', frame)
-            if cv2.waitKey(1) & 0xFF == ord('q'):
-                break
-        cap.release()
-        
-        # ffmpegcv use by camera name, in Windows&Linux
-        cap = ffmpegcv.VideoCaptureCAM("Integrated Camera")
-        
-        # ffmpegcv use camera path if multiple cameras conflict
-        cap = ffmpegcv.VideoCaptureCAM('@device_pnp_\\\\?\\usb#vid_2304&'
-            'pid_oot#media#0001#{65e8773d-8f56-11d0-a3b9-00a0c9223196}'
-            '\\global')
-        
-        # ffmpegcv use camera with ROI operations
-        cap = ffmpegcv.VideoCaptureCAM("Integrated Camera", crop_xywh=(0, 0, 640, 480), resize=(512, 512), resize_keepratio=True)
-        
-        
-        ```
-        
-        **list all camera devices**
-        ```python
-        from ffmpegcv.ffmpeg_reader_camera import query_camera_devices
-        
-        devices = query_camera_devices()
-        print(devices)
-        ```
-        >{0: ('Integrated Camera', '@device_pnp_\\\\?\\usb#vid_2304&pid_oot#media#0001#{65e8773d-8f56-11d0-a3b9-00a0c9223196}\\global'),  
-        1: ('OBS Virtual Camera', '@device_sw_{860BB310-5D01-11D0-BD3B-00A0C911CE86}\\{A3FCE0F5-3493-419F-958A-ABA1250EC20B}')}
-        
-        
-        **Set the camera resolution, fps, vcodec/pixel-format**
-        
-        ```python
-        from ffmpegcv.ffmpeg_reader_camera import query_camera_options
-        
-        options = query_camera_options(0)  # or query_camera_options("Integrated Camera") 
-        print(options)
-        cap = ffmpegcv.VideoCaptureCAM(0, **options[-1])
-        ```
-        >[{'camcodec': 'mjpeg', 'campix_fmt': None, 'camsize_wh': (1280, 720), 'camfps': 60.0002}, {'camcodec': 'mjpeg', 'campix_fmt': None, 'camsize_wh': (640, 480), 'camfps': 60.0002}, {'camcodec': 'mjpeg', 'campix_fmt': None, 'camsize_wh': (1920, 1080), 'camfps': 60.0002}, {'camcodec': None, 'campix_fmt': 'yuyv422', 'camsize_wh': (1280, 720), 'camfps': 10}, {'camcodec': None, 'campix_fmt': 'yuyv422', 'camsize_wh': (640, 480), 'camfps': 30}, {'camcodec': None, 'campix_fmt': 'yuyv422', 'camsize_wh': (1920, 1080), 'camfps': 5}]
-        
-        **Known issues**
-        1. The VideoCaptureCAM didn't give a smooth experience in macOS. You must specify all the camera parameters. And the query_camera_options woun't give any suggestion. That's because the `ffmpeg` cannot list device options using mac native `avfoundation`. 
-        ```python
-        # The macOS requires full argument.
-        cap = ffmpegcv.VideoCaptureCAM('FaceTime HD Camera', camsize_wh=(1280,720), camfps=30, campix_fmt='nv12')
-        ```
-        
-        2. The VideoCaptureCAM cann't list the FPS in linux. Because the `ffmpeg` cound't query the device's FPS using linux native `v4l2` module. However, it's just OK to let the FPS blank.
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# FFMPEGCV is an alternative to OPENCV for video read and write.
+The ffmpegcv provide Video Reader and Video Witer with ffmpeg backbone, which are faster and powerful than cv2.
+
+- The ffmpegcv is api **compatible** to open-cv. 
+- The ffmpegcv can use **GPU accelerate** encoding and decoding*. 
+- The ffmpegcv support much more video **codecs** v.s. open-cv.
+- The ffmpegcv support **RGB** & BGR format as you like.
+- The ffmpegcv can support ROI operations.You can **crop**, **resize** and **pad** the ROI.
+
+In all, ffmpegcv is just similar to opencv api. But is faster* and with more codecs.
+
+
+## Basic example
+Read a video by CPU, and rewrite it by GPU.
+```python
+vidin = ffmpegcv.VideoCapture(vfile_in)
+vidout = ffmpegcv.VideoWriterNV(vfile_out, 'h264', vidin.fps)
+
+with vidin, vidout:
+    for frame in vidin:
+        cv2.imshow('image', frame)
+        vidout.write(frame)
+```
+
+Read the camera by device name.
+```python
+cap = ffmpegcv.VideoCaptureCAM("Integrated Camera")
+```
+
+## Install
+You need to download ffmpeg before you can use ffmpegcv
+> conda install ffmpeg 
+>
+> pip install ffmpegcv
+
+## GPU Accelation
+- Support NVIDIA card only.
+- Perfect in the **Windows**. That ffmpeg supports NVIDIA acceleration just by conda install.
+- Struggle in the **Linux**. That ffmpeg didn't orginally support NVIDIA accelerate.
+Please re-compile the ffmpeg by yourself.
+See the [link](https://docs.nvidia.com/video-technologies/video-codec-sdk/ffmpeg-with-nvidia-gpu/)
+- Works in the **Google Colab** notebook without pain (no need to recompile ffmpeg). 
+- Infeasible in the **MacOS**. That ffmpeg didn't supports NVIDIA at all.
+
+> \* The ffmegcv GPU reader is a bit slower than CPU reader, but much faster when use ROI operations (crop, resize, pad).
+
+## Codecs
+
+| Codecs      | OpenCV-reader | ffmpegcv-cpu-r     | gpu-r  | OpenCV-writer | ffmpegcv-cpu-w     | gpu-w  |
+| ----------- | ------------- | ---------------- | ---- | ------------- | ---------------- | ---- |
+| h264        | √             | √                | √    | ×             | √                | √    |
+| h265 (hevc) | not sure      | √                | √    | ×             | √                | √    |
+| mjpeg       | √             | √                | ×    | √             | √                | ×    |
+| mpeg        | √             | √                | ×    | √             | √                | ×    |
+| others      | not sure      | ffmpeg -decoders | ×    | not sure      | ffmpeg -encoders | ×    |
+
+## Benchmark
+*On the way...*
+
+
+## Video Reader
+---
+The ffmpegcv is just similar to opencv in api.
+```python
+# open cv
+import cv2
+cap = cv2.VideoCapture(file)
+while True:
+    ret, frame = cap.read()
+    if not ret:
+        break
+    pass
+
+# ffmpegcv
+import ffmpegcv
+cap = ffmpegcv.VideoCapture(file)
+while True:
+    ret, frame = cap.read()
+    if not ret:
+        break
+    pass
+cap.release()
+
+# alternative
+cap = ffmpegcv.VideoCapture(file)
+nframe = len(cap)
+for frame in cap:
+    pass
+cap.release()
+
+# more pythonic, recommand
+with ffmpegcv.VideoCapture(file) as cap:
+    nframe = len(cap)
+    for iframe, frame in enumerate(cap):
+        if iframe>100: break
+        pass
+```
+
+Use GPU to accelerate decoding. It depends on the video codes.
+h264_nvcuvid, hevc_nvcuvid ....
+```python
+cap_cpu = ffmpegcv.VideoCapture(file)
+cap_gpu = ffmpegcv.VideoCapture(file, codec='h264_cuvid') #NVIDIA GPU0
+cap_gpu0 = ffmpegcv.VideoCaptureNV(file)         #NVIDIA GPU0
+cap_gpu1 = ffmpegcv.VideoCaptureNV(file, gpu=1)  #NVIDIA GPU1
+```
+
+Use rgb24 instead of bgr24
+```python
+cap = ffmpegcv.VideoCapture(file, pix_fmt='rgb24')
+ret, frame = cap.read()
+plt.imshow(frame)
+```
+
+### ROI Operations
+You can crop, resize and pad the video. These ROI operation is `ffmpegcv-GPU` > `ffmpegcv-CPU` >> `opencv`.
+
+**Crop** video, which will be much faster than read the whole canvas.
+```python
+cap = ffmpegcv.VideoCapture(file, crop_xywh=(0, 0, 640, 480))
+```
+
+**Resize** the video to the given size.
+```python
+cap = ffmpegcv.VideoCapture(file, resize=(640, 480))
+```
+
+**Resize** and keep the aspect ratio with black border **padding**.
+```python
+cap = ffmpegcv.VideoCapture(file, resize=(640, 480), resize_keepratio=True)
+```
+
+**Crop** and then **resize** the video.
+```python
+cap = ffmpegcv.VideoCapture(file, crop_xywh=(0, 0, 640, 480), resize=(512, 512))
+```
+
+## Video Writer
+---
+```python
+# cv2
+out = cv2.VideoWriter('outpy.avi',
+                       cv2.VideoWriter_fourcc('M','J','P','G'), 
+                       10, 
+                       (w, h))
+out.write(frame1)
+out.write(frame2)
+out.release()
+
+# ffmpegcv, default codec is 'h264' in cpu 'h265' in gpu.
+# frameSize is decided by the size of the first frame
+out = ffmpegcv.VideoWriter('outpy.mp4', None, 10)
+out.write(frame1)
+out.write(frame2)
+out.release()
+
+# more pythonic
+with ffmpegcv.VideoWriter('outpy.mp4', None, 10) as out:
+    out.write(frame1)
+    out.write(frame2)
+```
+
+
+Use GPU to accelerate encoding. Such as h264_nvenc, hevc_nvenc.
+```python
+out_cpu = ffmpegcv.VideoWriter('outpy.mp4', None, 10)
+out_gpu0 = ffmpegcv.VideoWriterNV('outpy.mp4', 'h264', 10)        #NVIDIA GPU0
+out_gpu1 = ffmpegcv.VideoWriterNV('outpy.mp4', 'hevc', 10, gpu=1) #NVIDIA GPU1
+```
+
+Input image is rgb24 instead of bgr24
+```python
+out = ffmpegcv.VideoWriter('outpy.mp4', None, 10, pix_fmt='rgb24')
+out.write(cv2.cvtColor(frame, cv2.COLOR_BGR2RGB))
+```
+
+## Video Reader and Writer
+---
+```python
+import ffmpegcv
+vfile_in = 'A.mp4'
+vfile_out = 'A_h264.mp4'
+vidin = ffmpegcv.VideoCapture(vfile_in)
+vidout = ffmpegcv.VideoWriter(vfile_out, None, vidin.fps)
+
+with vidin, vidout:
+    for frame in vidin:
+        vidout.write(frame)
+```
+
+## Camera Reader
+---
+**Experimental feature**. The ffmpegcv offers Camera reader. Which is consistent with VideoFiler reader. 
+
+- The `VideoCaptureCAM` aims to support ROI operations. The Opencv will be general fascinating than ffmpegcv in camera read. **I recommand the opencv in most camera reading case**.
+- The ffmpegcv can use name to retrieve the camera device. Use `ffmpegcv.VideoCaptureCAM("Integrated Camera")` is readable than `cv2.VideoCaptureCAM(0)`.
+- The `VideoCaptureCAM` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
+- The `VideoCaptureCAM` is continously working on background even if you didn't read it. Please release it in time.
+- Works perfect in Windows, not-perfect in Linux and macOS.
+
+```python
+import cv2
+cap = cv2.VideoCapture(0)
+while True:
+    ret, frame = cap.read()
+    cv2.imshow('frame', frame)
+    if cv2.waitKey(1) & 0xFF == ord('q'):
+        break
+cap.release()
+
+# ffmpegcv, in Windows&Linux
+import ffmpegcv
+cap = ffmpegcv.VideoCaptureCAM(0)
+while True:
+    ret, frame = cap.read()
+    cv2.imshow('frame', frame)
+    if cv2.waitKey(1) & 0xFF == ord('q'):
+        break
+cap.release()
+
+# ffmpegcv use by camera name, in Windows&Linux
+cap = ffmpegcv.VideoCaptureCAM("Integrated Camera")
+
+# ffmpegcv use camera path if multiple cameras conflict
+cap = ffmpegcv.VideoCaptureCAM('@device_pnp_\\\\?\\usb#vid_2304&'
+    'pid_oot#media#0001#{65e8773d-8f56-11d0-a3b9-00a0c9223196}'
+    '\\global')
+
+# ffmpegcv use camera with ROI operations
+cap = ffmpegcv.VideoCaptureCAM("Integrated Camera", crop_xywh=(0, 0, 640, 480), resize=(512, 512), resize_keepratio=True)
+
+
+```
+
+**list all camera devices**
+```python
+from ffmpegcv.ffmpeg_reader_camera import query_camera_devices
+
+devices = query_camera_devices()
+print(devices)
+```
+>{0: ('Integrated Camera', '@device_pnp_\\\\?\\usb#vid_2304&pid_oot#media#0001#{65e8773d-8f56-11d0-a3b9-00a0c9223196}\\global'),  
+1: ('OBS Virtual Camera', '@device_sw_{860BB310-5D01-11D0-BD3B-00A0C911CE86}\\{A3FCE0F5-3493-419F-958A-ABA1250EC20B}')}
+
+
+**Set the camera resolution, fps, vcodec/pixel-format**
+
+```python
+from ffmpegcv.ffmpeg_reader_camera import query_camera_options
+
+options = query_camera_options(0)  # or query_camera_options("Integrated Camera") 
+print(options)
+cap = ffmpegcv.VideoCaptureCAM(0, **options[-1])
+```
+>[{'camcodec': 'mjpeg', 'campix_fmt': None, 'camsize_wh': (1280, 720), 'camfps': 60.0002}, {'camcodec': 'mjpeg', 'campix_fmt': None, 'camsize_wh': (640, 480), 'camfps': 60.0002}, {'camcodec': 'mjpeg', 'campix_fmt': None, 'camsize_wh': (1920, 1080), 'camfps': 60.0002}, {'camcodec': None, 'campix_fmt': 'yuyv422', 'camsize_wh': (1280, 720), 'camfps': 10}, {'camcodec': None, 'campix_fmt': 'yuyv422', 'camsize_wh': (640, 480), 'camfps': 30}, {'camcodec': None, 'campix_fmt': 'yuyv422', 'camsize_wh': (1920, 1080), 'camfps': 5}]
+
+**Known issues**
+1. The VideoCaptureCAM didn't give a smooth experience in macOS. You must specify all the camera parameters. And the query_camera_options woun't give any suggestion. That's because the `ffmpeg` cannot list device options using mac native `avfoundation`. 
+```python
+# The macOS requires full argument.
+cap = ffmpegcv.VideoCaptureCAM('FaceTime HD Camera', camsize_wh=(1280,720), camfps=30, campix_fmt='nv12')
+```
+
+2. The VideoCaptureCAM cann't list the FPS in linux. Because the `ffmpeg` cound't query the device's FPS using linux native `v4l2` module. However, it's just OK to let the FPS blank.
+
+
+## Stream Reader
+**Experimental feature**. The ffmpegcv offers Camera reader. Which is consistent with VideoFiler reader. The feature is like a camera.
+Becareful when using it.
+
+- Support `RTSP`, `RTP`, `RTMP`, `HTTP`, `HTTPS` streams.
+- The `VideoCaptureStream` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
+- The `VideoCaptureStream` is continously working on background even if you didn't read it. Please release it in time.
+
+
+```python
+import cv2
+stream_url = 'http://devimages.apple.com.edgekey.net/streaming/examples/bipbop_4x3/gear2/prog_index.m3u8'
+cap = cv2.VideoCapture(stream_url, cv2.CAP_FFMPEG)
+
+if not cap.isOpened():
+    print('Cannot open the stream')
+    exit(-1)
+
+while True:
+    ret, frame = cap.read()
+    if not ret:
+        break
+    pass
+
+# ffmpegcv, in Windows&Linux
+import ffmpegcv
+cap = ffmpegcv.VideoCaptureStream(stream_url)
+while True:
+    ret, frame = cap.read()
+    if not ret:
+        break
+    pass
+```
```

### Comparing `ffmpegcv-0.3.0/README.md` & `ffmpegcv-0.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: ffmpegcv
+Version: 0.3.1
+Home-page: https://pypi.org/project/ffmpegcv/
+Author: chenxf
+Author-email: cxf529125853@163.com
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # FFMPEGCV is an alternative to OPENCV for video read and write.
 The ffmpegcv provide Video Reader and Video Witer with ffmpeg backbone, which are faster and powerful than cv2.
 
 - The ffmpegcv is api **compatible** to open-cv. 
 - The ffmpegcv can use **GPU accelerate** encoding and decoding*. 
 - The ffmpegcv support much more video **codecs** v.s. open-cv.
 - The ffmpegcv support **RGB** & BGR format as you like.
@@ -186,15 +195,15 @@
 with vidin, vidout:
     for frame in vidin:
         vidout.write(frame)
 ```
 
 ## Camera Reader
 ---
-***Experimental feature**. The ffmpegcv offers Camera reader. Which is consistent with VideoFiler reader. 
+**Experimental feature**. The ffmpegcv offers Camera reader. Which is consistent with VideoFiler reader. 
 
 - The `VideoCaptureCAM` aims to support ROI operations. The Opencv will be general fascinating than ffmpegcv in camera read. **I recommand the opencv in most camera reading case**.
 - The ffmpegcv can use name to retrieve the camera device. Use `ffmpegcv.VideoCaptureCAM("Integrated Camera")` is readable than `cv2.VideoCaptureCAM(0)`.
 - The `VideoCaptureCAM` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
 - The `VideoCaptureCAM` is continously working on background even if you didn't read it. Please release it in time.
 - Works perfect in Windows, not-perfect in Linux and macOS.
 
@@ -258,7 +267,42 @@
 1. The VideoCaptureCAM didn't give a smooth experience in macOS. You must specify all the camera parameters. And the query_camera_options woun't give any suggestion. That's because the `ffmpeg` cannot list device options using mac native `avfoundation`. 
 ```python
 # The macOS requires full argument.
 cap = ffmpegcv.VideoCaptureCAM('FaceTime HD Camera', camsize_wh=(1280,720), camfps=30, campix_fmt='nv12')
 ```
 
 2. The VideoCaptureCAM cann't list the FPS in linux. Because the `ffmpeg` cound't query the device's FPS using linux native `v4l2` module. However, it's just OK to let the FPS blank.
+
+
+## Stream Reader
+**Experimental feature**. The ffmpegcv offers Camera reader. Which is consistent with VideoFiler reader. The feature is like a camera.
+Becareful when using it.
+
+- Support `RTSP`, `RTP`, `RTMP`, `HTTP`, `HTTPS` streams.
+- The `VideoCaptureStream` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
+- The `VideoCaptureStream` is continously working on background even if you didn't read it. Please release it in time.
+
+
+```python
+import cv2
+stream_url = 'http://devimages.apple.com.edgekey.net/streaming/examples/bipbop_4x3/gear2/prog_index.m3u8'
+cap = cv2.VideoCapture(stream_url, cv2.CAP_FFMPEG)
+
+if not cap.isOpened():
+    print('Cannot open the stream')
+    exit(-1)
+
+while True:
+    ret, frame = cap.read()
+    if not ret:
+        break
+    pass
+
+# ffmpegcv, in Windows&Linux
+import ffmpegcv
+cap = ffmpegcv.VideoCaptureStream(stream_url)
+while True:
+    ret, frame = cap.read()
+    if not ret:
+        break
+    pass
+```
```

### Comparing `ffmpegcv-0.3.0/ffmpegcv/__init__.py` & `ffmpegcv-0.3.1/ffmpegcv/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,71 @@
 from .ffmpeg_reader import FFmpegReader, FFmpegReaderNV
 from .ffmpeg_writer import FFmpegWriter, FFmpegWriterNV
 from .ffmpeg_reader_camera import FFmpegReaderCAM
+from .ffmpeg_reader_stream import FFmpegReaderStream
 from .video_info import get_num_NVIDIA_GPUs
 import shutil
 from subprocess import DEVNULL, check_output
 
 
 def _check():
-    if not shutil.which('ffmpeg') or not shutil.which('ffprobe'):
-        raise RuntimeError('The ffmpeg is not installed. \n\n'
-                           'Please install ffmpeg via:\n    '
-                           'conda install ffmpeg')
+    if not shutil.which("ffmpeg") or not shutil.which("ffprobe"):
+        raise RuntimeError(
+            "The ffmpeg is not installed. \n\n"
+            "Please install ffmpeg via:\n    "
+            "conda install ffmpeg"
+        )
+
 
 _check()
 
 _check_nvidia_init = None
 
+
 def _check_nvidia():
     global _check_nvidia_init
     run = lambda x: check_output(x, shell=True, stderr=DEVNULL)
     if _check_nvidia_init is None:
-        calling_output = run('ffmpeg -h encoder=hevc_nvenc')
-        if 'AVOptions' not in calling_output.decode('utf-8'):
-            raise RuntimeError('The ffmpeg is not compiled with NVENC support.\n\n'
-                               'Please re-compile ffmpeg following the instructions at:\n    '
-                               'https://docs.nvidia.com/video-technologies/video-codec-sdk/ffmpeg-with-nvidia-gpu/')
-
-        calling_output = run('ffmpeg -h decoder=hevc_cuvid')
-        if 'AVOptions' not in calling_output.decode('utf-8'):
-            raise RuntimeError('The ffmpeg is not compiled with NVENC support.\n\n'
-                               'Please re-compile ffmpeg following the instructions at:\n    '
-                               'https://docs.nvidia.com/video-technologies/video-codec-sdk/ffmpeg-with-nvidia-gpu/')
+        calling_output = run("ffmpeg -h encoder=hevc_nvenc")
+        if "AVOptions" not in calling_output.decode("utf-8"):
+            raise RuntimeError(
+                "The ffmpeg is not compiled with NVENC support.\n\n"
+                "Please re-compile ffmpeg following the instructions at:\n    "
+                "https://docs.nvidia.com/video-technologies/video-codec-sdk/ffmpeg-with-nvidia-gpu/"
+            )
+
+        calling_output = run("ffmpeg -h decoder=hevc_cuvid")
+        if "AVOptions" not in calling_output.decode("utf-8"):
+            raise RuntimeError(
+                "The ffmpeg is not compiled with NVENC support.\n\n"
+                "Please re-compile ffmpeg following the instructions at:\n    "
+                "https://docs.nvidia.com/video-technologies/video-codec-sdk/ffmpeg-with-nvidia-gpu/"
+            )
 
         if get_num_NVIDIA_GPUs() == 0:
-            raise RuntimeError('No NVIDIA GPU found.\n\n'
-                               'Please use a NVIDIA GPU card listed at:\n    '
-                               'https://developer.nvidia.com/video-encode-and-decode-gpu-support-matrix-new')
+            raise RuntimeError(
+                "No NVIDIA GPU found.\n\n"
+                "Please use a NVIDIA GPU card listed at:\n    "
+                "https://developer.nvidia.com/video-encode-and-decode-gpu-support-matrix-new"
+            )
 
         _check_nvidia_init = True
 
     return True
 
 
-def VideoCapture(file, 
-                 codec=None, 
-                 pix_fmt='bgr24',
-                 crop_xywh=None,
-                 resize=None,
-                 resize_keepratio=True,
-                 resize_keepratioalign='center'):
+def VideoCapture(
+    file,
+    codec=None,
+    pix_fmt="bgr24",
+    crop_xywh=None,
+    resize=None,
+    resize_keepratio=True,
+    resize_keepratioalign="center",
+):
     """
     Alternative to cv2.VideoCapture
 
     Parameters
     ----------
     file : str
         Path to video file.
@@ -121,57 +134,54 @@
     cap = ffmpegcv.VideoCapture(file, resize=(640, 480))
     ```
 
     Resize and keep the aspect ratio with black border
     ```
     cap = ffmpegcv.VideoCapture(file, resize=(640, 480), resize_keepratio=True)
     ```
-    
+
     Crop and then resize the video.
     ```python
     cap = ffmpegcv.VideoCapture(file, crop_xywh=(0, 0, 640, 480), resize=(512, 512))
     ```
     Author: Chenxinfeng 2022-04-16, cxf529125853@163.com
     """
-    return FFmpegReader.VideoReader(file, codec, pix_fmt, crop_xywh,
-                                    resize, resize_keepratio, resize_keepratioalign)
+    return FFmpegReader.VideoReader(
+        file, codec, pix_fmt, crop_xywh, resize, resize_keepratio, resize_keepratioalign
+    )
 
 
-VideoReader=VideoCapture                                                                 
+VideoReader = VideoCapture
 
 
-def VideoWriter(file, 
-                codec=None, 
-                fps=30, 
-                frameSize=None, 
-                pix_fmt='bgr24'):
+def VideoWriter(file, codec=None, fps=30, frameSize=None, pix_fmt="bgr24"):
     """
     Alternative to cv2.VideoWriter
 
     Parameters
     ----------
     file : str
         Path to video file.
     codec : str
         Codec to use. Optional. Default is `None` (x264).
     fps : number
         Frames per second. Optional. Default is 30.
     frameSize : tuple
-        Frame size. (width, height). Optional. Default is `None`, which is 
+        Frame size. (width, height). Optional. Default is `None`, which is
         decided by the size of the first frame.
     pix_fmt : str
         Pixel format of input. ['bgr24' | 'rgb24']. Optional. Default is 'bgr24'.
 
     Examples
     --------
     opencv
     ```
     out = cv2.VideoWriter('outpy.avi',
-                          cv2.VideoWriter_fourcc('M','J','P','G'), 
-                          10, 
+                          cv2.VideoWriter_fourcc('M','J','P','G'),
+                          10,
                           (w, h))
     out.write(frame1)
     out.write(frame2)
     out.release()
     ```
 
     ffmpegcv
@@ -200,53 +210,192 @@
     ```
 
     Author: Chenxinfeng 2022-04-16, cxf529125853@163.com
     """
     return FFmpegWriter.VideoWriter(file, codec, fps, frameSize, pix_fmt)
 
 
-def VideoCaptureNV(file,
-                   pix_fmt='bgr24',
-                   crop_xywh=None,
-                   resize=None,
-                   resize_keepratio=True,
-                   resize_keepratioalign='center',
-                   gpu=0):
+def VideoCaptureNV(
+    file,
+    pix_fmt="bgr24",
+    crop_xywh=None,
+    resize=None,
+    resize_keepratio=True,
+    resize_keepratioalign="center",
+    gpu=0,
+):
     """
     `ffmpegcv.VideoCaptureNV` is a gpu version for `ffmpegcv.VideoCapture`.
     """
     _check_nvidia()
-    return FFmpegReaderNV.VideoReader(file, pix_fmt, crop_xywh, 
-                                      resize, resize_keepratio, resize_keepratioalign, 
-                                      gpu)
+    return FFmpegReaderNV.VideoReader(
+        file, pix_fmt, crop_xywh, resize, resize_keepratio, resize_keepratioalign, gpu
+    )
+
 
 VideoReaderNV = VideoCaptureNV
 
-def VideoWriterNV(file,
-                  codec=None,
-                  fps=30,
-                  frameSize=None,
-                  pix_fmt='bgr24',
-                  gpu=0):
+
+def VideoWriterNV(file, codec=None, fps=30, frameSize=None, pix_fmt="bgr24", gpu=0):
     """
     `ffmpegcv.VideoWriterNV` is a gpu version for `ffmpegcv.VideoWriter`.
     """
     _check_nvidia()
     return FFmpegWriterNV.VideoWriter(file, codec, fps, frameSize, pix_fmt, gpu)
 
 
-def VideoCaptureCAM(camname,
-                    pix_fmt='bgr24',
-                    crop_xywh=None,
-                    resize=None,
-                    resize_keepratio=True,
-                    resize_keepratioalign='center',
-                    camsize_wh=None,
-                    camfps=None,
-                    camcodec=None,
-                    campix_fmt=None):
-    return FFmpegReaderCAM.VideoReader(camname, pix_fmt, crop_xywh,
-        resize, resize_keepratio, resize_keepratioalign,
-        camsize_wh=camsize_wh, camfps=camfps, camcodec=camcodec,
-        campix_fmt=campix_fmt)
+def VideoCaptureCAM(
+    camname,
+    pix_fmt="bgr24",
+    crop_xywh=None,
+    resize=None,
+    resize_keepratio=True,
+    resize_keepratioalign="center",
+    camsize_wh=None,
+    camfps=None,
+    camcodec=None,
+    campix_fmt=None,
+):
+    """
+    Alternative to cv2.VideoCapture
+
+    Parameters
+    ----------
+    file : see ffmpegcv.VideoReader
+    codec : see ffmpegcv.VideoReader
+    pix_fmt : see ffmpegcv.VideoReader
+    crop_xywh : see ffmpegcv.VideoReader
+    resize  : see ffmpegcv.VideoReader
+    resize_keepratio : see ffmpegcv.VideoReader
+    resize_keepratioalign : see ffmpegcv.VideoReader
+    camsize_wh: tuple or None
+        Camera resolution (width, height). e.g (800, 600)
+    camfps: float or None
+        Camera framerate. e.g. 30.
+    camcodec: str or None
+        Camera codec. e.g. 'mjpeg' or 'h264'.
+    campix_fmt: str or None
+        Camera pixel format. e.g. 'rgb24' or 'yuv420p'.
+        Just set one of `camcodec` or `campix_fmt`.
+    Examples
+    --------
+    opencv
+    ```
+    cap = cv2.VideoCapture(0)
+    while True:
+        ret, frame = cap.read()
+        if not ret:
+            break
+        pass
+    ```
+
+    ffmpegcv
+    ```
+    cap = ffmpegcv.VideoCaptureCAM(0)
+    while True:
+        ret, frame = cap.read()
+        if not ret:
+            break
+        pass
+    ```
+
+    Or use camera name
+    ```
+    cap = ffmpegcv.VideoCaptureCAM("Integrated Camera")
+    ```
+
+    Use full camera parameter
+    ```
+    cap = ffmpegcv.VideoCaptureCAM('FaceTime HD Camera', 
+                                    camsize_wh = (1280,720), 
+                                    camfps = 30, 
+                                    campix_fmt = 'nv12')
+    ```
+
+    Use camera with ROI operations
+    ```
+    cap = ffmpegcv.VideoCaptureCAM("Integrated Camera", 
+                                    crop_xywh = (0, 0, 640, 480), 
+                                    resize = (512, 512), 
+                                    resize_keepratio = True)
+    ```
+    Author: Chenxinfeng 2023-05-11, cxf529125853@163.com
+    """
+    return FFmpegReaderCAM.VideoReader(
+        camname,
+        pix_fmt,
+        crop_xywh,
+        resize,
+        resize_keepratio,
+        resize_keepratioalign,
+        camsize_wh=camsize_wh,
+        camfps=camfps,
+        camcodec=camcodec,
+        campix_fmt=campix_fmt,
+    )
+
 
 VideoReaderCAM = VideoCaptureCAM
+
+
+def VideoCaptureStream(
+    stream_url,
+    pix_fmt="bgr24",
+    crop_xywh=None,
+    resize=None,
+    resize_keepratio=True,
+    resize_keepratioalign="center"
+):
+    """
+    Alternative to cv2.VideoCapture
+
+    Parameters
+    ----------
+    stream_url : RTSP, RTP, RTMP, HTTP, HTTPS url
+    codec : see ffmpegcv.VideoReader
+    pix_fmt : see ffmpegcv.VideoReader
+    crop_xywh : see ffmpegcv.VideoReader
+    resize  : see ffmpegcv.VideoReader
+    resize_keepratio : see ffmpegcv.VideoReader
+    resize_keepratioalign : see ffmpegcv.VideoReader
+
+    Examples
+    --------
+    opencv
+    ```
+    stream_url = 'http://devimages.apple.com.edgekey.net/streaming/examples/bipbop_4x3/gear2/prog_index.m3u8'
+    cap = cv2.VideoCapture(stream_url, cv2.CAP_FFMPEG)
+
+    if not cap.isOpened():
+        print('Cannot open the stream')
+        exit(-1)
+
+    while True:
+        ret, frame = cap.read()
+        if not ret:
+            break
+        pass
+    ```
+
+    ffmpegcv
+    ```
+    cap = ffmpegcv.VideoCaptureStream(stream_url)
+    while True:
+        ret, frame = cap.read()
+        if not ret:
+            break
+        pass
+    ```
+
+    Author: Chenxinfeng 2023-05-31, cxf529125853@163.com
+    """
+    return FFmpegReaderStream.VideoReader(
+        stream_url,
+        pix_fmt,
+        crop_xywh,
+        resize,
+        resize_keepratio,
+        resize_keepratioalign
+    )
+
+
+VideoReaderStream = VideoCaptureStream
```

### Comparing `ffmpegcv-0.3.0/ffmpegcv/ffmpeg_reader.py` & `ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import numpy as np
 import pprint
 import os
-from .video_info import (run_async, get_info, get_num_NVIDIA_GPUs, 
-                        decoder_to_nvidia, release_process)
+from .video_info import (
+    run_async,
+    get_info,
+    get_num_NVIDIA_GPUs,
+    decoder_to_nvidia,
+    release_process,
+)
 
 
 class FFmpegReader:
     def __init__(self):
         self.iframe = -1
 
     def __repr__(self):
-        props = pprint.pformat(self.__dict__).replace('{',' ').replace('}',' ')
-        return f'{self.__class__}\n'  + props
+        props = pprint.pformat(self.__dict__).replace("{", " ").replace("}", " ")
+        return f"{self.__class__}\n" + props
 
     def __enter__(self):
         return self
-    
+
     def __exit__(self, type, value, traceback):
         self.release()
 
     def __len__(self):
         return self.count
 
     def __iter__(self):
@@ -29,91 +34,115 @@
         ret, img = self.read()
         if ret:
             return img
         else:
             raise StopIteration
 
     @staticmethod
-    def VideoReader(filename, codec, pix_fmt, crop_xywh,
-                    resize, resize_keepratio, resize_keepratioalign):
-        assert os.path.exists(filename) and os.path.isfile(filename), f'{filename} not exists'
-        assert pix_fmt in ['rgb24', 'bgr24', 'yuv420p', 'nv12']
+    def VideoReader(
+        filename,
+        codec,
+        pix_fmt,
+        crop_xywh,
+        resize,
+        resize_keepratio,
+        resize_keepratioalign,
+    ):
+        assert os.path.exists(filename) and os.path.isfile(
+            filename
+        ), f"{filename} not exists"
+        assert pix_fmt in ["rgb24", "bgr24", "yuv420p", "nv12"]
 
         vid = FFmpegReader()
         videoinfo = get_info(filename)
         vid.width = videoinfo.width
         vid.height = videoinfo.height
         vid.fps = videoinfo.fps
         vid.count = videoinfo.count
         vid.origin_width, vid.origin_height = vid.width, vid.height
         vid.codec = codec if codec else videoinfo.codec
         if crop_xywh:
             crop_w, crop_h = crop_xywh[2:]
             vid.width, vid.height = crop_w, crop_h
             x, y, w, h = crop_xywh
-            cropopt = f'crop={w}:{h}:{x}:{y}'
+            cropopt = f"crop={w}:{h}:{x}:{y}"
         else:
             crop_w, crop_h = vid.origin_width, vid.origin_height
-            cropopt = ''
+            cropopt = ""
 
         vid.crop_width, vid.crop_height = crop_w, crop_h
 
         if resize is None or resize == (vid.crop_width, vid.crop_height):
-            scaleopt = ''
-            padopt = ''
+            scaleopt = ""
+            padopt = ""
         else:
             vid.width, vid.height = dst_width, dst_height = resize
             if not resize_keepratio:
-                scaleopt = f'scale={dst_width}x{dst_height}'
-                padopt = ''
+                scaleopt = f"scale={dst_width}x{dst_height}"
+                padopt = ""
             else:
-                re_width, re_height = crop_w/(crop_h / dst_height) , dst_height
+                re_width, re_height = crop_w / (crop_h / dst_height), dst_height
                 if re_width > dst_width:
-                    re_width, re_height = dst_width, crop_h/(crop_w / dst_width)
+                    re_width, re_height = dst_width, crop_h / (crop_w / dst_width)
                 re_width, re_height = int(re_width), int(re_height)
-                scaleopt = f'scale={re_width}x{re_height}'
-                if resize_keepratioalign is None: resize_keepratioalign = 'center'
-                paddings = {'center': ((dst_width - re_width) // 2, (dst_height - re_height) // 2),
-                            'topleft': (0, 0),
-                            'topright': (dst_width - re_width, 0),
-                            'bottomleft': (0, dst_height - re_height), 
-                            'bottomright': (dst_width - re_width, dst_height - re_height)}
-                assert resize_keepratioalign in paddings, 'resize_keepratioalign must be one of "center"(mmpose), "topleft"(mmdetection), "topright", "bottomleft", "bottomright"'
+                scaleopt = f"scale={re_width}x{re_height}"
+                if resize_keepratioalign is None:
+                    resize_keepratioalign = "center"
+                paddings = {
+                    "center": (
+                        (dst_width - re_width) // 2,
+                        (dst_height - re_height) // 2,
+                    ),
+                    "topleft": (0, 0),
+                    "topright": (dst_width - re_width, 0),
+                    "bottomleft": (0, dst_height - re_height),
+                    "bottomright": (dst_width - re_width, dst_height - re_height),
+                }
+                assert (
+                    resize_keepratioalign in paddings
+                ), 'resize_keepratioalign must be one of "center"(mmpose), "topleft"(mmdetection), "topright", "bottomleft", "bottomright"'
                 xpading, ypading = paddings[resize_keepratioalign]
-                padopt = f'pad={dst_width}:{dst_height}:{xpading}:{ypading}:black'
-        
+                padopt = f"pad={dst_width}:{dst_height}:{xpading}:{ypading}:black"
+
         if any([cropopt, scaleopt, padopt]):
-            filterstr = ','.join(x for x in [cropopt, scaleopt, padopt] if x)
-            filteropt = f'-vf {filterstr}'
+            filterstr = ",".join(x for x in [cropopt, scaleopt, padopt] if x)
+            filteropt = f"-vf {filterstr}"
         else:
-            filteropt = ''
+            filteropt = ""
 
-        args = (f'ffmpeg -loglevel warning '
-                f' -vcodec {vid.codec} -r {vid.fps} -i "{filename}" '
-                f' {filteropt} -pix_fmt {pix_fmt} -r {vid.fps} -f rawvideo pipe:')
+        args = (
+            f"ffmpeg -loglevel warning "
+            f' -vcodec {vid.codec} -r {vid.fps} -i "{filename}" '
+            f" {filteropt} -pix_fmt {pix_fmt} -r {vid.fps} -f rawvideo pipe:"
+        )
 
         vid.process = run_async(args)
         vid.size = (vid.width, vid.height)
         vid.pix_fmt = pix_fmt
-        assert (not pix_fmt=='yuv420p') or (vid.height % 2 == 0 and vid.width % 2 == 0), 'yuv420p must be even'
-        vid.out_numpy_shape = {'rgb24': (vid.height, vid.width, 3),
-                            'bgr24': (vid.height, vid.width, 3),
-                            'nv12': (int(vid.height * 1.5), vid.width),
-                            'yuv420p': (int(vid.height * 1.5), vid.width)}[pix_fmt]
+        assert (not pix_fmt == "yuv420p") or (
+            vid.height % 2 == 0 and vid.width % 2 == 0
+        ), "yuv420p must be even"
+        vid.out_numpy_shape = {
+            "rgb24": (vid.height, vid.width, 3),
+            "bgr24": (vid.height, vid.width, 3),
+            "nv12": (int(vid.height * 1.5), vid.width),
+            "yuv420p": (int(vid.height * 1.5), vid.width),
+        }[pix_fmt]
         return vid
 
     def read_gray(self):
         # It's an experimental function
         # return 'ret, img_gray'
         # img_gray: Height x Width x 1
-        assert self.pix_fmt in ('nv12', 'yuv420p')
+        assert self.pix_fmt in ("nv12", "yuv420p")
         ret, img = self.read()
-        if not ret: return False, None
-        assert img.shape==(int(self.height * 1.5), self.width)
-        img_gray = img[:self.height, :, None]
+        if not ret:
+            return False, None
+        assert img.shape == (int(self.height * 1.5), self.width)
+        img_gray = img[: self.height, :, None]
         return True, img_gray
 
     def read(self):
         in_bytes = self.process.stdout.read(np.prod(self.out_numpy_shape))
         if not in_bytes:
             self.release()
             return False, None
@@ -126,85 +155,116 @@
         release_process(self.process)
 
     def close(self):
         return self.release()
 
 
 class FFmpegReaderNV(FFmpegReader):
-    def _get_opts(vid, videoinfo, crop_xywh, resize, 
-                  resize_keepratio, resize_keepratioalign):
+    def _get_opts(
+        vid, videoinfo, crop_xywh, resize, resize_keepratio, resize_keepratioalign
+    ):
         vid.origin_width = videoinfo.width
         vid.origin_height = videoinfo.height
         vid.fps = videoinfo.fps
         vid.count = videoinfo.count
         vid.width, vid.height = vid.origin_width, vid.origin_height
         vid.codec = videoinfo.codec
-        assert vid.origin_height %2 == 0, 'height must be even'
-        assert vid.origin_width %2 == 0, 'width must be even'
+        assert vid.origin_height % 2 == 0, "height must be even"
+        assert vid.origin_width % 2 == 0, "width must be even"
         if crop_xywh:
             crop_w, crop_h = crop_xywh[2:]
             vid.width, vid.height = crop_w, crop_h
             x, y, w, h = crop_xywh
-            top, bottom, left, right = y, vid.origin_height - (y + h), x, vid.origin_width - (x + w)  #crop length
-            cropopt = f'-crop {top}x{bottom}x{left}x{right}'
+            top, bottom, left, right = (
+                y,
+                vid.origin_height - (y + h),
+                x,
+                vid.origin_width - (x + w),
+            )  # crop length
+            cropopt = f"-crop {top}x{bottom}x{left}x{right}"
         else:
             crop_w, crop_h = vid.origin_width, vid.origin_height
-            cropopt = ''
+            cropopt = ""
 
         vid.crop_width, vid.crop_height = crop_w, crop_h
 
         if resize is None or resize == (vid.crop_width, vid.crop_height):
-            scaleopt = ''
-            filteropt = ''
+            scaleopt = ""
+            filteropt = ""
         else:
             vid.width, vid.height = dst_width, dst_height = resize
             if not resize_keepratio:
-                scaleopt = f'-resize {dst_width}x{dst_height}'
-                filteropt = ''
+                scaleopt = f"-resize {dst_width}x{dst_height}"
+                filteropt = ""
             else:
-                re_width, re_height = crop_w/(crop_h / dst_height) , dst_height
+                re_width, re_height = crop_w / (crop_h / dst_height), dst_height
                 if re_width > dst_width:
-                    re_width, re_height = dst_width, crop_h/(crop_w / dst_width)
+                    re_width, re_height = dst_width, crop_h / (crop_w / dst_width)
                 re_width, re_height = int(re_width), int(re_height)
-                scaleopt = f'-resize {re_width}x{re_height}'
-                if resize_keepratioalign is None: resize_keepratioalign = 'center'
-                paddings = {'center': ((dst_width - re_width) // 2, (dst_height - re_height) // 2),
-                            'topleft': (0, 0),
-                            'topright': (dst_width - re_width, 0),
-                            'bottomleft': (0, dst_height - re_height), 
-                            'bottomright': (dst_width - re_width, dst_height - re_height)}
-                assert resize_keepratioalign in paddings, 'resize_keepratioalign must be one of "center"(mmpose), "topleft"(mmdetection), "topright", "bottomleft", "bottomright"'
+                scaleopt = f"-resize {re_width}x{re_height}"
+                if resize_keepratioalign is None:
+                    resize_keepratioalign = "center"
+                paddings = {
+                    "center": (
+                        (dst_width - re_width) // 2,
+                        (dst_height - re_height) // 2,
+                    ),
+                    "topleft": (0, 0),
+                    "topright": (dst_width - re_width, 0),
+                    "bottomleft": (0, dst_height - re_height),
+                    "bottomright": (dst_width - re_width, dst_height - re_height),
+                }
+                assert (
+                    resize_keepratioalign in paddings
+                ), 'resize_keepratioalign must be one of "center"(mmpose), "topleft"(mmdetection), "topright", "bottomleft", "bottomright"'
                 xpading, ypading = paddings[resize_keepratioalign]
-                padopt = f'pad={dst_width}:{dst_height}:{xpading}:{ypading}:black'
-                filteropt = f'-vf {padopt}'
+                padopt = f"pad={dst_width}:{dst_height}:{xpading}:{ypading}:black"
+                filteropt = f"-vf {padopt}"
 
         vid.size = (vid.width, vid.height)
         return cropopt, scaleopt, filteropt
 
     @staticmethod
-    def VideoReader(filename, pix_fmt, crop_xywh, 
-                    resize, resize_keepratio, resize_keepratioalign, 
-                    gpu):
-        assert os.path.exists(filename) and os.path.isfile(filename), f'{filename} not exists'
-        assert pix_fmt in ['rgb24', 'bgr24', 'yuv420p', 'nv12']
+    def VideoReader(
+        filename,
+        pix_fmt,
+        crop_xywh,
+        resize,
+        resize_keepratio,
+        resize_keepratioalign,
+        gpu,
+    ):
+        assert os.path.exists(filename) and os.path.isfile(
+            filename
+        ), f"{filename} not exists"
+        assert pix_fmt in ["rgb24", "bgr24", "yuv420p", "nv12"]
         numGPU = get_num_NVIDIA_GPUs()
-        assert numGPU>0, 'No GPU found'
+        assert numGPU > 0, "No GPU found"
         gpu = int(gpu) % numGPU if gpu is not None else 0
-        assert resize is None or len(resize) == 2, 'resize must be a tuple of (width, height)'
+        assert (
+            resize is None or len(resize) == 2
+        ), "resize must be a tuple of (width, height)"
         videoinfo = get_info(filename)
         vid = FFmpegReaderNV()
-        cropopt, scaleopt, filteropt = vid._get_opts(videoinfo, crop_xywh, resize, 
-            resize_keepratio, resize_keepratioalign)
+        cropopt, scaleopt, filteropt = vid._get_opts(
+            videoinfo, crop_xywh, resize, resize_keepratio, resize_keepratioalign
+        )
         vid.codecNV = decoder_to_nvidia(vid.codec)
 
-        args = (f'ffmpeg -loglevel warning -hwaccel cuda -hwaccel_device {gpu} '
-                f' -vcodec {vid.codecNV} {cropopt} {scaleopt} -r {vid.fps} -i "{filename}" '
-                f' {filteropt} -pix_fmt {pix_fmt} -r {vid.fps} -f rawvideo pipe:')
+        args = (
+            f"ffmpeg -loglevel warning -hwaccel cuda -hwaccel_device {gpu} "
+            f' -vcodec {vid.codecNV} {cropopt} {scaleopt} -r {vid.fps} -i "{filename}" '
+            f" {filteropt} -pix_fmt {pix_fmt} -r {vid.fps} -f rawvideo pipe:"
+        )
 
         vid.process = run_async(args)
         vid.pix_fmt = pix_fmt
-        assert (not pix_fmt=='yuv420p') or (vid.height % 2 == 0 and vid.width % 2 == 0), 'yuv420p must be even'
-        vid.out_numpy_shape = {'rgb24': (vid.height, vid.width, 3),
-                            'bgr24': (vid.height, vid.width, 3),
-                            'yuv420p': (int(vid.height * 1.5), vid.width),
-                            'nv12': (int(vid.height * 1.5), vid.width)}[pix_fmt]
+        assert (not pix_fmt == "yuv420p") or (
+            vid.height % 2 == 0 and vid.width % 2 == 0
+        ), "yuv420p must be even"
+        vid.out_numpy_shape = {
+            "rgb24": (vid.height, vid.width, 3),
+            "bgr24": (vid.height, vid.width, 3),
+            "yuv420p": (int(vid.height * 1.5), vid.width),
+            "nv12": (int(vid.height * 1.5), vid.width),
+        }[pix_fmt]
         return vid
```

### Comparing `ffmpegcv-0.3.0/ffmpegcv/ffmpeg_reader_camera.py` & `ffmpegcv-0.3.1/ffmpegcv/ffmpeg_reader_camera.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,228 +1,272 @@
 import numpy as np
 import pprint
-from .video_info import (run_async, release_process)
+from .video_info import run_async, release_process
 import re
 import subprocess
 from threading import Thread
 from queue import Queue
 import sys
+import os
 
 
-class platform():
+class platform:
     win = 0
     linux = 1
     mac = 2
     other = 3
 
-if sys.platform.startswith('linux'):
+
+if sys.platform.startswith("linux"):
     this_os = platform.linux
-elif sys.platform.startswith('win32'):
+elif sys.platform.startswith("win32"):
     this_os = platform.win
-elif sys.platform.startswith('darwin'):
+elif sys.platform.startswith("darwin"):
     this_os = platform.mac
 else:
     this_os = platform.other
 
 
 def _query_camera_divices_mac() -> dict:
     # run the command 'ffmpeg -f avfoundation -list_devices true -i "" '
     command = 'ffmpeg -hide_banner -f avfoundation -list_devices true -i ""'
-    process = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    process = subprocess.Popen(
+        command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
+    )
     stdout, stderr = process.communicate()
 
     # parse the output into a dictionary
-    lines = stderr.decode('utf-8').split('AVFoundation audio devices:')[0].split('\n')
+    lines = stderr.decode("utf-8").split("AVFoundation audio devices:")[0].split("\n")
     id_device_map = dict()
-    device_id_pattern = re.compile(r'\[[^\]]*?\] \[(\d*)\]')
-    device_name_pattern = re.compile(r'.*\] (.*)')
+    device_id_pattern = re.compile(r"\[[^\]]*?\] \[(\d*)\]")
+    device_name_pattern = re.compile(r".*\] (.*)")
     for line in lines[1:-1]:
         device_id = int(re.search(device_id_pattern, line).group(1))
         device_name = re.search(device_name_pattern, line).group(1)
         id_device_map[device_id] = (device_name, device_id)
     return id_device_map
 
 
 def _query_camera_divices_win() -> dict:
-    command = 'ffmpeg -hide_banner -list_devices true -f dshow -i dummy'
+    command = "ffmpeg -hide_banner -list_devices true -f dshow -i dummy"
     process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     stdout, stderr = process.communicate()
-    dshowliststr = stderr.decode('utf-8')
-    dshowliststr = dshowliststr.split('DirectShow audio devices')[0]
+    dshowliststr = stderr.decode("utf-8")
+    dshowliststr = dshowliststr.split("DirectShow audio devices")[0]
     pattern = re.compile(r'\[[^\]]*?\]  "([^"]*)"')
     matches = pattern.findall(dshowliststr)
     alternative_pattern = re.compile(r'Alternative name "(.*)"')
     alternative_names = alternative_pattern.findall(dshowliststr)
-    assert len(matches)==len(alternative_names)
-    id_device_map = {i:device for i, device in enumerate(zip(matches, alternative_names))}
-    if len(id_device_map)==0:
-        print('No camera divice found')
+    assert len(matches) == len(alternative_names)
+    id_device_map = {
+        i: device for i, device in enumerate(zip(matches, alternative_names))
+    }
+    if len(id_device_map) == 0:
+        print("No camera divice found")
     return id_device_map
 
 
 def _query_camera_divices_linux() -> dict:
     "edit from https://github.com/p513817/python-get-cam-name/blob/master/get_cam_name.py"
-    import os    
     root = "/sys/class/video4linux"
-    cam_info=[]
-    
-    for index in sorted([file for file in os.listdir(root)]):        
+    cam_info = []
+
+    for index in sorted([file for file in os.listdir(root)]):
         # Get Camera Name From /sys/class/video4linux/<video*>/name
         real_index_file = os.path.realpath("/sys/class/video4linux/" + index + "/index")
         with open(real_index_file, "r") as name_file:
             _index = name_file.read().rstrip()
-            if _index != '0':
+            if _index != "0":
                 continue
 
         real_file = os.path.realpath("/sys/class/video4linux/" + index + "/name")
         with open(real_file, "r") as name_file:
             name = name_file.read().rstrip()
-            name = name.split(':')[0]
-        
-        # Setup Each Camera and Index ( video* )    
-        cam_info.append((name, '/dev/'+index))
+            name = name.split(":")[0]
 
-    id_device_map = {i:vname for i, vname in enumerate(cam_info)}
+        # Setup Each Camera and Index ( video* )
+        cam_info.append((name, "/dev/" + index))
+
+    id_device_map = {i: vname for i, vname in enumerate(cam_info)}
     return id_device_map
 
 
 def query_camera_devices(verbose_dict: bool = False) -> dict:
-    result = {platform.linux: _query_camera_divices_linux,
-            platform.mac: _query_camera_divices_mac,
-            platform.win: _query_camera_divices_win}[this_os]()
+    result = {
+        platform.linux: _query_camera_divices_linux,
+        platform.mac: _query_camera_divices_mac,
+        platform.win: _query_camera_divices_win,
+    }[this_os]()
     if verbose_dict:
-        dict_by_v0 = {v[0]:v for v in result.values()}
-        dict_by_v1 = {v[1]:v for v in result.values()}
+        dict_by_v0 = {v[0]: v for v in result.values()}
+        dict_by_v1 = {v[1]: v for v in result.values()}
         result.update(dict_by_v0)
         result.update(dict_by_v1)
-    
+
     return result
-            
+
 
 def _query_camera_options_mac(cam_id_name) -> str:
-    print('\033[33m' + "FFmpeg& FFmpegcv CAN NOT query the camera options in MAC platform."+ '\033[0m')
-    print('Please find the proper parameter other way.')
-    return [{'camsize_wh':None, 'camfps':None}]
+    print(
+        "\033[33m"
+        + "FFmpeg& FFmpegcv CAN NOT query the camera options in MAC platform."
+        + "\033[0m"
+    )
+    print("Please find the proper parameter other way.")
+    return [{"camsize_wh": None, "camfps": None}]
 
 
 def _query_camera_options_linux(cam_id_name) -> str:
-    print('\033[33m' + "FFmpeg& FFmpegcv CAN NOT query the camera FPS in Linux platform."+ '\033[0m')
-    print('Please find the proper parameter other way.')
-    camname = query_camera_devices(verbose_dict=True)[cam_id_name][1] 
+    print(
+        "\033[33m"
+        + "FFmpeg& FFmpegcv CAN NOT query the camera FPS in Linux platform."
+        + "\033[0m"
+    )
+    print("Please find the proper parameter other way.")
+    camname = query_camera_devices(verbose_dict=True)[cam_id_name][1]
     command = f'ffmpeg -hide_banner -f v4l2 -list_formats all -i "{camname}"'
-    process = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    process = subprocess.Popen(
+        command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
+    )
     stdout, stderr = process.communicate()
-    lines = stderr.decode('utf-8').split('\n')
-    lines = [l for l in lines if 'v4l2' in l]
+    lines = stderr.decode("utf-8").split("\n")
+    lines = [l for l in lines if "v4l2" in l]
     outlist = []
     for line in lines:
-        _, vcodec, *_, resolutions = line.split(':')
+        _, vcodec, *_, resolutions = line.split(":")
         vcodec = vcodec.strip()
-        israw = 'Raw'in line
+        israw = "Raw" in line
         camcodec = None if israw else vcodec
         campix_fmt = vcodec if israw else None
         resolutions = resolutions.strip()
 
-        camsize_wh_l = [tuple(map(int, r.split('x'))) for r in resolutions.split()]
-        outlist.extend([{'camcodec':camcodec, 'campix_fmt':campix_fmt, 'camsize_wh':wh, 'camfps':None} 
-                        for wh in camsize_wh_l])
+        camsize_wh_l = [tuple(map(int, r.split("x"))) for r in resolutions.split()]
+        outlist.extend(
+            [
+                {
+                    "camcodec": camcodec,
+                    "campix_fmt": campix_fmt,
+                    "camsize_wh": wh,
+                    "camfps": None,
+                }
+                for wh in camsize_wh_l
+            ]
+        )
     return outlist
 
 
 def _query_camera_options_win(cam_id_name) -> str:
     if isinstance(cam_id_name, int):
         id_device_map = query_camera_devices()
         camname = id_device_map[cam_id_name][1]
     elif isinstance(cam_id_name, str):
         camname = cam_id_name
     else:
-        raise ValueError('Not valid camname')
+        raise ValueError("Not valid camname")
     command = f'ffmpeg -hide_banner -f dshow -list_options true -i video="{camname}"'
     process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     stdout, stderr = process.communicate()
-    dshowliststr = stderr.decode('utf-8').replace('\r\n','\n').replace('\r', '\n')
-    dshowlist = [s for s in dshowliststr.split('\n') if 'fps=' in s]
+    dshowliststr = stderr.decode("utf-8").replace("\r\n", "\n").replace("\r", "\n")
+    dshowlist = [s for s in dshowliststr.split("\n") if "fps=" in s]
     from collections import OrderedDict
+
     unique_dshowlist = list(OrderedDict.fromkeys(dshowlist))
     outlist = []
     for text in unique_dshowlist:
         cam_options = dict()
-        cam_options['camcodec'] = re.search(r"vcodec=(\w+)", text).group(1) if 'vcodec' in text else None
-        cam_options['campix_fmt'] = re.search(r"pixel_format=(\w+)", text).group(1) if 'pixel_format' in text else None
+        cam_options["camcodec"] = (
+            re.search(r"vcodec=(\w+)", text).group(1) if "vcodec" in text else None
+        )
+        cam_options["campix_fmt"] = (
+            re.search(r"pixel_format=(\w+)", text).group(1)
+            if "pixel_format" in text
+            else None
+        )
         camsize_wh = re.search(r"min s=(\w+)", text).group(1)
-        cam_options['camsize_wh'] = tuple(int(v) for v in camsize_wh.split('x'))
-        camfps = float(re.findall(r'fps=([\d.]+)', text)[-1])
-        cam_options['camfps'] = int(camfps) if int(camfps)==camfps else camfps
+        cam_options["camsize_wh"] = tuple(int(v) for v in camsize_wh.split("x"))
+        camfps = float(re.findall(r"fps=([\d.]+)", text)[-1])
+        cam_options["camfps"] = int(camfps) if int(camfps) == camfps else camfps
         outlist.append(cam_options)
     return outlist
 
 
 def query_camera_options(cam_id_name) -> str:
-    return {platform.linux: _query_camera_options_linux,
+    return {
+        platform.linux: _query_camera_options_linux,
         platform.mac: _query_camera_options_mac,
-        platform.win: _query_camera_options_win}[this_os](cam_id_name)
+        platform.win: _query_camera_options_win,
+    }[this_os](cam_id_name)
 
 
 class ProducerThread(Thread):
     def __init__(self, vid, q):
-        super(ProducerThread,self).__init__()
+        super(ProducerThread, self).__init__()
         self.vid = vid
         self.q = q
 
     def run(self):
         while True:
             if not self.vid.isopened:
                 break
             ret, img = self.vid.read_()
 
             try:
-                self.q.put_nowait((ret, img)) #drop frames 
+                self.q.put_nowait((ret, img))  # drop frames
             except Exception:
                 pass
             continue
 
 
 class FFmpegReaderCAM:
     def __init__(self):
         self.iframe = -1
 
     def __repr__(self):
-        props = pprint.pformat(self.__dict__).replace('{',' ').replace('}',' ')
-        return f'{self.__class__}\n'  + props
+        props = pprint.pformat(self.__dict__).replace("{", " ").replace("}", " ")
+        return f"{self.__class__}\n" + props
 
     def __enter__(self):
         return self
-    
+
     def __exit__(self, type, value, traceback):
         self.release()
 
     def __iter__(self):
         return self
 
     def __next__(self):
         ret, img = self.read()
         if ret:
             return img
         else:
             raise StopIteration
 
     @staticmethod
-    def VideoReader(cam_id_name, pix_fmt, crop_xywh,
-                    resize, resize_keepratio, resize_keepratioalign,
-                    camsize_wh=None, camfps=None, camcodec=None, 
-                    campix_fmt=None, step=1):
-        assert pix_fmt in ['rgb24', 'bgr24', 'yuv420p', 'nv12']
+    def VideoReader(
+        cam_id_name,
+        pix_fmt,
+        crop_xywh,
+        resize,
+        resize_keepratio,
+        resize_keepratioalign,
+        camsize_wh=None,
+        camfps=None,
+        camcodec=None,
+        campix_fmt=None,
+        step=1,
+    ):
+        assert pix_fmt in ["rgb24", "bgr24", "yuv420p", "nv12"]
 
         vid = FFmpegReaderCAM()
         if this_os == platform.mac:
             # use cam_id as the device marker
             if isinstance(cam_id_name, str):
                 id_device_map = query_camera_devices()
                 camname = cam_id_name
-                id_device_map.update({v[0]:v for v in id_device_map.values()})
+                id_device_map.update({v[0]: v for v in id_device_map.values()})
                 camid = id_device_map[cam_id_name][1]
             else:
                 camname = None
                 camid = cam_id_name
         elif this_os == platform.linux:
             id_device_map = query_camera_devices(verbose_dict=True)
             camname = id_device_map[cam_id_name][-1]
@@ -237,133 +281,155 @@
                 camid = None
 
         vid.camname = camname
         vid.camid = camid
 
         if camsize_wh is None:
             cam_options = query_camera_options(camname)
-            resolutions = [c['camsize_wh'] for c in cam_options]
+            resolutions = [c["camsize_wh"] for c in cam_options]
             camsize_wh = max(resolutions, key=lambda x: sum(x))
 
-        assert len(camsize_wh)==2
+        assert len(camsize_wh) == 2
         vid.width, vid.height = camsize_wh
-        
-        opt_camfps = f' -framerate {camfps} ' if camfps else ''
+
+        opt_camfps = f" -framerate {camfps} " if camfps else ""
         vid.camfps = camfps if camfps else None
 
-        opt_camcodec_ = {platform.linux: 'input_format',
-                        platform.mac: '',
-                        platform.win: 'vcodec'}[this_os]
-        opt_camcodec = f' -{opt_camcodec_} {camcodec} ' if camcodec else ''
+        opt_camcodec_ = {
+            platform.linux: "input_format",
+            platform.mac: "",
+            platform.win: "vcodec",
+        }[this_os]
+        opt_camcodec = f" -{opt_camcodec_} {camcodec} " if camcodec else ""
         vid.camcodec = camcodec if camcodec else None
 
-        opt_campix_fmt_ = {platform.linux: 'input_format',
-                        platform.mac: 'pixel_format',
-                        platform.win: 'pixel_format'}[this_os]
-        opt_campix_fmt = f' -{opt_campix_fmt_} {campix_fmt} ' if campix_fmt else ''
+        opt_campix_fmt_ = {
+            platform.linux: "input_format",
+            platform.mac: "pixel_format",
+            platform.win: "pixel_format",
+        }[this_os]
+        opt_campix_fmt = f" -{opt_campix_fmt_} {campix_fmt} " if campix_fmt else ""
         vid.campix_fmt = campix_fmt if campix_fmt else None
 
-        opt_camname = {platform.linux: f'"{camname}"',
-                       platform.win: f'video="{camname}"',
-                       platform.mac: f'{camid}:none'}[this_os]
+        opt_camname = {
+            platform.linux: f'"{camname}"',
+            platform.win: f'video="{camname}"',
+            platform.mac: f"{camid}:none",
+        }[this_os]
 
         vid.origin_width, vid.origin_height = vid.width, vid.height
         if crop_xywh:
             crop_w, crop_h = crop_xywh[2:]
             vid.width, vid.height = crop_w, crop_h
             x, y, w, h = crop_xywh
-            cropopt = f'crop={w}:{h}:{x}:{y}'
+            cropopt = f"crop={w}:{h}:{x}:{y}"
         else:
             crop_w, crop_h = vid.origin_width, vid.origin_height
-            cropopt = ''
+            cropopt = ""
 
         vid.crop_width, vid.crop_height = crop_w, crop_h
 
         if resize is None or resize == (vid.crop_width, vid.crop_height):
-            scaleopt = ''
-            padopt = ''
+            scaleopt = ""
+            padopt = ""
         else:
             vid.width, vid.height = dst_width, dst_height = resize
             if not resize_keepratio:
-                scaleopt = f'scale={dst_width}x{dst_height}'
-                padopt = ''
+                scaleopt = f"scale={dst_width}x{dst_height}"
+                padopt = ""
             else:
-                re_width, re_height = crop_w/(crop_h / dst_height) , dst_height
+                re_width, re_height = crop_w / (crop_h / dst_height), dst_height
                 if re_width > dst_width:
-                    re_width, re_height = dst_width, crop_h/(crop_w / dst_width)
+                    re_width, re_height = dst_width, crop_h / (crop_w / dst_width)
                 re_width, re_height = int(re_width), int(re_height)
-                scaleopt = f'scale={re_width}x{re_height}'
-                if resize_keepratioalign is None: resize_keepratioalign = 'center'
-                paddings = {'center': ((dst_width - re_width) // 2, (dst_height - re_height) // 2),
-                            'topleft': (0, 0),
-                            'topright': (dst_width - re_width, 0),
-                            'bottomleft': (0, dst_height - re_height), 
-                            'bottomright': (dst_width - re_width, dst_height - re_height)}
-                assert resize_keepratioalign in paddings, 'resize_keepratioalign must be one of "center"(mmpose), "topleft"(mmdetection), "topright", "bottomleft", "bottomright"'
+                scaleopt = f"scale={re_width}x{re_height}"
+                if resize_keepratioalign is None:
+                    resize_keepratioalign = "center"
+                paddings = {
+                    "center": (
+                        (dst_width - re_width) // 2,
+                        (dst_height - re_height) // 2,
+                    ),
+                    "topleft": (0, 0),
+                    "topright": (dst_width - re_width, 0),
+                    "bottomleft": (0, dst_height - re_height),
+                    "bottomright": (dst_width - re_width, dst_height - re_height),
+                }
+                assert (
+                    resize_keepratioalign in paddings
+                ), 'resize_keepratioalign must be one of "center"(mmpose), "topleft"(mmdetection), "topright", "bottomleft", "bottomright"'
                 xpading, ypading = paddings[resize_keepratioalign]
-                padopt = f'pad={dst_width}:{dst_height}:{xpading}:{ypading}:black'
-        
+                padopt = f"pad={dst_width}:{dst_height}:{xpading}:{ypading}:black"
+
         if any([cropopt, scaleopt, padopt]):
-            filterstr = ','.join(x for x in [cropopt, scaleopt, padopt] if x)
-            filteropt = f'-vf {filterstr}'
+            filterstr = ",".join(x for x in [cropopt, scaleopt, padopt] if x)
+            filteropt = f"-vf {filterstr}"
         else:
-            filteropt = ''
+            filteropt = ""
 
-        opt_driver_ = {platform.linux: 'v4l2',
-                        platform.mac: 'avfoundation',
-                        platform.win: 'dshow'}[this_os]
-        
-        args = (f'ffmpeg -loglevel warning '
-                f' -f {opt_driver_} '
-                f' -video_size {vid.origin_width}x{vid.origin_height} '
-                f' {opt_camfps} {opt_camcodec} {opt_campix_fmt} '
-                f' -i {opt_camname} '
-                f' {filteropt} -pix_fmt {pix_fmt} -f rawvideo pipe:')
+        opt_driver_ = {
+            platform.linux: "v4l2",
+            platform.mac: "avfoundation",
+            platform.win: "dshow",
+        }[this_os]
+
+        args = (
+            f"ffmpeg -loglevel warning "
+            f" -f {opt_driver_} "
+            f" -video_size {vid.origin_width}x{vid.origin_height} "
+            f" {opt_camfps} {opt_camcodec} {opt_campix_fmt} "
+            f" -i {opt_camname} "
+            f" {filteropt} -pix_fmt {pix_fmt} -f rawvideo pipe:"
+        )
 
         vid.size = (vid.width, vid.height)
         vid.pix_fmt = pix_fmt
-        assert (not pix_fmt=='yuv420p') or (vid.height % 2 == 0 and vid.width % 2 == 0), 'yuv420p must be even'
-        vid.out_numpy_shape = {'rgb24': (vid.height, vid.width, 3),
-                            'bgr24': (vid.height, vid.width, 3),
-                            'yuv420p': (int(vid.height * 1.5), vid.width),
-                            'nv12': (int(vid.height * 1.5), vid.width),
-                            }[pix_fmt]
+        assert (not pix_fmt == "yuv420p") or (
+            vid.height % 2 == 0 and vid.width % 2 == 0
+        ), "yuv420p must be even"
+        vid.out_numpy_shape = {
+            "rgb24": (vid.height, vid.width, 3),
+            "bgr24": (vid.height, vid.width, 3),
+            "yuv420p": (int(vid.height * 1.5), vid.width),
+            "nv12": (int(vid.height * 1.5), vid.width),
+        }[pix_fmt]
         vid.process = run_async(args)
 
         vid.isopened = True
-        
+
         # producer
-        assert step>=1 and isinstance(step, int)
-        vid.step=step
+        assert step >= 1 and isinstance(step, int)
+        vid.step = step
         vid.q = Queue(maxsize=30)
         producer = ProducerThread(vid, vid.q)
         producer.start()
         return vid
 
     def read_(self):
         for i in range(self.step):
             in_bytes = self.process.stdout.read(np.prod(self.out_numpy_shape))
         if not in_bytes:
             self.release()
             return False, None
-        
+
         self.iframe += 1
         img = None
         img = np.frombuffer(in_bytes, np.uint8).reshape(self.out_numpy_shape)
         return True, img
-    
+
     def read_gray(self):
         # It's an experimental function
         # return 'ret, img_gray'
         # img_gray: Height x Width x 1
-        assert self.pix_fmt in ('nv12', 'yuv420p')
+        assert self.pix_fmt in ("nv12", "yuv420p")
         ret, img = self.read()
-        if not ret: return False, None
-        assert img.shape==(int(self.height * 1.5), self.width)
-        img_gray = img[:self.height, :, None]
+        if not ret:
+            return False, None
+        assert img.shape == (int(self.height * 1.5), self.width)
+        img_gray = img[: self.height, :, None]
         return True, img_gray
 
     def read(self):
         ret, img = self.q.get()
         return ret, img
 
     def release(self):
```

### Comparing `ffmpegcv-0.3.0/ffmpegcv/ffmpeg_writer.py` & `ffmpegcv-0.3.1/ffmpegcv/ffmpeg_writer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,105 +1,116 @@
 import numpy as np
 import warnings
 import pprint
 import sys
 from .video_info import run_async, release_process, get_num_NVIDIA_GPUs
 
 
-IN_COLAB = 'google.colab' in sys.modules
+IN_COLAB = "google.colab" in sys.modules
 
 
 class FFmpegWriter:
     def __init__(self):
         self.iframe = -1
 
     def __enter__(self):
         return self
-    
+
     def __exit__(self, type, value, traceback):
         self.release()
 
     def __del__(self):
         self.release()
 
     def __repr__(self):
-        props = pprint.pformat(self.__dict__).replace('{',' ').replace('}',' ')
-        return f'{self.__class__}\n'  + props
+        props = pprint.pformat(self.__dict__).replace("{", " ").replace("}", " ")
+        return f"{self.__class__}\n" + props
 
     @staticmethod
-    def VideoWriter(filename, codec, fps, frameSize, pix_fmt):
+    def VideoWriter(filename, codec, fps, frameSize, pix_fmt, bitrate=None):
         if codec is None:
-            codec = 'h264'
+            codec = "h264"
         elif not isinstance(codec, str):
-            codec = 'h264'
-            warnings.simplefilter('''
+            codec = "h264"
+            warnings.simplefilter(
+                """
                 Codec should be a string. Eg `h264`, `h264_nvenc`. 
                 You may used CV2.VideoWriter_fourcc, which will be ignored.
-                ''')
-        
+                """
+            )
+
         vid = FFmpegWriter()
         vid.fps, vid.size = fps, frameSize
         vid.width, vid.height = vid.size if vid.size else (None, None)
         vid.codec, vid.pix_fmt, vid.filename = codec, pix_fmt, filename
         vid.waitInit = True
+        vid.bitrate = bitrate
         return vid
 
     def _init_video_stream(self):
+        bitrate_str = f'-b:v {self.bitrate} ' if self.bitrate else ''
         args = (f'ffmpeg -y -loglevel warning ' 
                 f'-f rawvideo -pix_fmt {self.pix_fmt} -s {self.width}x{self.height} -r {self.fps} -i pipe: '
+                f'{bitrate_str} '
                 f'-r {self.fps} -c:v {self.codec} -pix_fmt yuv420p "{self.filename}"')
         self.process = run_async(args)
 
     def write(self, img):
         if self.waitInit:
             if self.size is None:
-                self.size = (img.shape[1], img.shape[0])          
+                self.size = (img.shape[1], img.shape[0])
             self.width, self.height = self.size
             self._init_video_stream()
             self.waitInit = False
-        
+
         self.iframe += 1
         assert self.size == (img.shape[1], img.shape[0])
         img = img.astype(np.uint8).tobytes()
         self.process.stdin.write(img)
 
     def release(self):
-        if hasattr(self, 'process'):
+        if hasattr(self, "process"):
             release_process(self.process)
 
     def close(self):
         return self.release()
 
 
 class FFmpegWriterNV(FFmpegWriter):
     @staticmethod
-    def VideoWriter(filename, codec, fps, frameSize, pix_fmt, gpu):
+    def VideoWriter(filename, codec, fps, frameSize, pix_fmt, gpu, bitrate=None):
         numGPU = get_num_NVIDIA_GPUs()
         assert numGPU
         gpu = int(gpu) % numGPU if gpu is not None else 0
         if codec is None:
-            codec = 'hevc_nvenc'
+            codec = "hevc_nvenc"
         elif not isinstance(codec, str):
-            codec = 'hevc_nvenc'
-            warnings.simplefilter('''
+            codec = "hevc_nvenc"
+            warnings.simplefilter(
+                """
                 Codec should be a string. Eg `h264`, `h264_nvenc`. 
                 You may used CV2.VideoWriter_fourcc, which will be ignored.
-                ''')
-        elif codec.endswith('_nvenc'):
+                """
+            )
+        elif codec.endswith("_nvenc"):
             codec = codec
         else:
-            codec = codec + '_nvenc'
-        assert codec in ['hevc_nvenc', 'h264_nvenc'], 'codec should be `hevc_nvenc` or `h264_nvenc`'
+            codec = codec + "_nvenc"
+        assert codec in [
+            "hevc_nvenc",
+            "h264_nvenc",
+        ], "codec should be `hevc_nvenc` or `h264_nvenc`"
 
         vid = FFmpegWriterNV()
         vid.fps, vid.size = fps, frameSize
         vid.width, vid.height = vid.size if vid.size else (None, None)
         vid.codec, vid.pix_fmt, vid.filename = codec, pix_fmt, filename
         vid.gpu = gpu
         vid.waitInit = True
+        vid.bitrate = bitrate
         return vid
 
     def _init_video_stream(self):
         default_preset = 'default' if IN_COLAB else 'p2'
         self.preset = getattr(self, 'preset', default_preset)
         args = (f'ffmpeg -y -loglevel warning '
             f'-f rawvideo -pix_fmt {self.pix_fmt} -s {self.width}x{self.height} -r {self.fps} -i pipe: '
```

### Comparing `ffmpegcv-0.3.0/ffmpegcv/video_info.py` & `ffmpegcv-0.3.1/ffmpegcv/video_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,89 +2,95 @@
 from subprocess import Popen, PIPE
 import re
 from collections import namedtuple
 import xml.etree.ElementTree as ET
 
 
 def get_info(video):
-    cmd = 'ffprobe -v quiet -print_format xml -select_streams v:0 -show_format -show_streams "{}"'.format(video)
+    cmd = 'ffprobe -v quiet -print_format xml -select_streams v:0 -count_packets -show_format -show_streams "{}"'.format(video)
     output = subprocess.check_output(cmd, shell=True)
     root = ET.fromstring(output)
-    assert (root[0].tag, root[0][0].tag) == ('streams', 'stream')
+    assert (root[0].tag, root[0][0].tag) == ("streams", "stream")
     vinfo = root[0][0].attrib
 
-    VideoInfo = namedtuple('VideoInfo', ['width', 'height', 'fps', 'count', 
-                                        'codec', 'duration'])
+    VideoInfo = namedtuple(
+        "VideoInfo", ["width", "height", "fps", "count", "codec", "duration"]
+    )
     outinfo = dict()
     outinfo['width'] = int(vinfo['width'])
     outinfo['height'] = int(vinfo['height'])
     outinfo['fps'] = eval(vinfo['r_frame_rate'])
-    outinfo['count'] = int(vinfo['nb_frames'])
+    outinfo['count'] = int(vinfo['nb_read_packets']) #nb_read_packets | nb_frames
     outinfo['codec'] = vinfo['codec_name']
     outinfo['duration'] = float(vinfo['duration'])
     videoinfo = VideoInfo(**outinfo)
 
     return videoinfo
 
 
 def get_num_NVIDIA_GPUs():
-    cmd = 'ffmpeg -f lavfi -i nullsrc -c:v h264_nvenc -gpu list -f null -'
+    cmd = "ffmpeg -f lavfi -i nullsrc -c:v h264_nvenc -gpu list -f null -"
     p = Popen(cmd.split(), shell=False, stdin=PIPE, stdout=PIPE, stderr=PIPE)
     stdout, stderr = p.communicate(b"")
     p.stdin.close()
     p.stdout.close()
     p.terminate()
-    pattern = re.compile(r'GPU #\d+ - < ')
+    pattern = re.compile(r"GPU #\d+ - < ")
     nv_info = pattern.findall(stderr.decode())
     num_gpu = len(nv_info)
     return num_gpu
 
 
 def encoder_to_nvidia(codec):
-    codec_map = {'h264'      : 'h264_nvenc',
-                 'hevc'      : 'hevc_nvenc'}
+    codec_map = {"h264": "h264_nvenc", "hevc": "hevc_nvenc"}
 
     if codec in codec_map:
         return codec_map[codec]
     elif codec in codec_map.values():
         return codec
     else:
-        raise Exception('No NV codec found for %s' % codec)
-    
+        raise Exception("No NV codec found for %s" % codec)
+
 
 def decoder_to_nvidia(codec):
-    codec_map = {'av1'       : 'av1_cuvid',
-                 'h264'      : 'h264_cuvid',
-                 'x264'      : 'h264_cuvid',    
-                 'hevc'      : 'hevc_cuvid',
-                 'x265'      : 'hevc_cuvid',
-                 'h265'      : 'hevc_cuvid',
-                 'mjpeg'     : 'mjpeg_cuvid',
-                 'mpeg1video': 'mpeg1_cuvid',
-                 'mpeg2video': 'mpeg2_cuvid',
-                 'mpeg4'     : 'mpeg4_cuvid',
-                 'vp1'       : 'vp1_cuvid',
-                 'vp8'       : 'vp8_cuvid',
-                 'vp9'       : 'vp9_cuvid'}
-    
+    codec_map = {
+        "av1": "av1_cuvid",
+        "h264": "h264_cuvid",
+        "x264": "h264_cuvid",
+        "hevc": "hevc_cuvid",
+        "x265": "hevc_cuvid",
+        "h265": "hevc_cuvid",
+        "mjpeg": "mjpeg_cuvid",
+        "mpeg1video": "mpeg1_cuvid",
+        "mpeg2video": "mpeg2_cuvid",
+        "mpeg4": "mpeg4_cuvid",
+        "vp1": "vp1_cuvid",
+        "vp8": "vp8_cuvid",
+        "vp9": "vp9_cuvid",
+    }
+
     if codec in codec_map:
         return codec_map[codec]
     elif codec in codec_map.values():
         return codec
     else:
-        raise Exception('No NV codec found for %s' % codec)
+        raise Exception("No NV codec found for %s" % codec)
 
 
 def run_async(args):
     quiet = True
     stderr_stream = subprocess.DEVNULL if quiet else None
     bufsize = -1
     return Popen(
-        args, stdin=PIPE, stdout=PIPE, stderr=stderr_stream, 
-        shell=isinstance(args, str), bufsize=bufsize
+        args,
+        stdin=PIPE,
+        stdout=PIPE,
+        stderr=stderr_stream,
+        shell=isinstance(args, str),
+        bufsize=bufsize,
     )
 
 
 def release_process(process):
     process.stdin.close()
     process.stdout.close()
     process.terminate()
```

### Comparing `ffmpegcv-0.3.0/ffmpegcv.egg-info/PKG-INFO` & `ffmpegcv-0.3.1/ffmpegcv.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,275 +1,308 @@
 Metadata-Version: 2.1
 Name: ffmpegcv
-Version: 0.3.0
-Summary: UNKNOWN
+Version: 0.3.1
 Home-page: https://pypi.org/project/ffmpegcv/
 Author: chenxf
 Author-email: cxf529125853@163.com
-License: UNKNOWN
-Description: # FFMPEGCV is an alternative to OPENCV for video read and write.
-        The ffmpegcv provide Video Reader and Video Witer with ffmpeg backbone, which are faster and powerful than cv2.
-        
-        - The ffmpegcv is api **compatible** to open-cv. 
-        - The ffmpegcv can use **GPU accelerate** encoding and decoding*. 
-        - The ffmpegcv support much more video **codecs** v.s. open-cv.
-        - The ffmpegcv support **RGB** & BGR format as you like.
-        - The ffmpegcv can support ROI operations.You can **crop**, **resize** and **pad** the ROI.
-        
-        In all, ffmpegcv is just similar to opencv api. But is faster* and with more codecs.
-        
-        
-        ## Basic example
-        Read a video by CPU, and rewrite it by GPU.
-        ```python
-        vidin = ffmpegcv.VideoCapture(vfile_in)
-        vidout = ffmpegcv.VideoWriterNV(vfile_out, 'h264', vidin.fps)
-        
-        with vidin, vidout:
-            for frame in vidin:
-                cv2.imshow('image', frame)
-                vidout.write(frame)
-        ```
-        
-        Read the camera by device name.
-        ```python
-        cap = ffmpegcv.VideoCaptureCAM("Integrated Camera")
-        ```
-        
-        ## Install
-        You need to download ffmpeg before you can use ffmpegcv
-        > conda install ffmpeg 
-        >
-        > pip install ffmpegcv
-        
-        ## GPU Accelation
-        - Support NVIDIA card only.
-        - Perfect in the **Windows**. That ffmpeg supports NVIDIA acceleration just by conda install.
-        - Struggle in the **Linux**. That ffmpeg didn't orginally support NVIDIA accelerate.
-        Please re-compile the ffmpeg by yourself.
-        See the [link](https://docs.nvidia.com/video-technologies/video-codec-sdk/ffmpeg-with-nvidia-gpu/)
-        - Works in the **Google Colab** notebook without pain (no need to recompile ffmpeg). 
-        - Infeasible in the **MacOS**. That ffmpeg didn't supports NVIDIA at all.
-        
-        > \* The ffmegcv GPU reader is a bit slower than CPU reader, but much faster when use ROI operations (crop, resize, pad).
-        
-        ## Codecs
-        
-        | Codecs      | OpenCV-reader | ffmpegcv-cpu-r     | gpu-r  | OpenCV-writer | ffmpegcv-cpu-w     | gpu-w  |
-        | ----------- | ------------- | ---------------- | ---- | ------------- | ---------------- | ---- |
-        | h264        | √             | √                | √    | ×             | √                | √    |
-        | h265 (hevc) | not sure      | √                | √    | ×             | √                | √    |
-        | mjpeg       | √             | √                | ×    | √             | √                | ×    |
-        | mpeg        | √             | √                | ×    | √             | √                | ×    |
-        | others      | not sure      | ffmpeg -decoders | ×    | not sure      | ffmpeg -encoders | ×    |
-        
-        ## Benchmark
-        *On the way...*
-        
-        
-        ## Video Reader
-        ---
-        The ffmpegcv is just similar to opencv in api.
-        ```python
-        # open cv
-        import cv2
-        cap = cv2.VideoCapture(file)
-        while True:
-            ret, frame = cap.read()
-            if not ret:
-                break
-            pass
-        
-        # ffmpegcv
-        import ffmpegcv
-        cap = ffmpegcv.VideoCapture(file)
-        while True:
-            ret, frame = cap.read()
-            if not ret:
-                break
-            pass
-        cap.release()
-        
-        # alternative
-        cap = ffmpegcv.VideoCapture(file)
-        nframe = len(cap)
-        for frame in cap:
-            pass
-        cap.release()
-        
-        # more pythonic, recommand
-        with ffmpegcv.VideoCapture(file) as cap:
-            nframe = len(cap)
-            for iframe, frame in enumerate(cap):
-                if iframe>100: break
-                pass
-        ```
-        
-        Use GPU to accelerate decoding. It depends on the video codes.
-        h264_nvcuvid, hevc_nvcuvid ....
-        ```python
-        cap_cpu = ffmpegcv.VideoCapture(file)
-        cap_gpu = ffmpegcv.VideoCapture(file, codec='h264_cuvid') #NVIDIA GPU0
-        cap_gpu0 = ffmpegcv.VideoCaptureNV(file)         #NVIDIA GPU0
-        cap_gpu1 = ffmpegcv.VideoCaptureNV(file, gpu=1)  #NVIDIA GPU1
-        ```
-        
-        Use rgb24 instead of bgr24
-        ```python
-        cap = ffmpegcv.VideoCapture(file, pix_fmt='rgb24')
-        ret, frame = cap.read()
-        plt.imshow(frame)
-        ```
-        
-        ### ROI Operations
-        You can crop, resize and pad the video. These ROI operation is `ffmpegcv-GPU` > `ffmpegcv-CPU` >> `opencv`.
-        
-        **Crop** video, which will be much faster than read the whole canvas.
-        ```python
-        cap = ffmpegcv.VideoCapture(file, crop_xywh=(0, 0, 640, 480))
-        ```
-        
-        **Resize** the video to the given size.
-        ```python
-        cap = ffmpegcv.VideoCapture(file, resize=(640, 480))
-        ```
-        
-        **Resize** and keep the aspect ratio with black border **padding**.
-        ```python
-        cap = ffmpegcv.VideoCapture(file, resize=(640, 480), resize_keepratio=True)
-        ```
-        
-        **Crop** and then **resize** the video.
-        ```python
-        cap = ffmpegcv.VideoCapture(file, crop_xywh=(0, 0, 640, 480), resize=(512, 512))
-        ```
-        
-        ## Video Writer
-        ---
-        ```python
-        # cv2
-        out = cv2.VideoWriter('outpy.avi',
-                               cv2.VideoWriter_fourcc('M','J','P','G'), 
-                               10, 
-                               (w, h))
-        out.write(frame1)
-        out.write(frame2)
-        out.release()
-        
-        # ffmpegcv, default codec is 'h264' in cpu 'h265' in gpu.
-        # frameSize is decided by the size of the first frame
-        out = ffmpegcv.VideoWriter('outpy.mp4', None, 10)
-        out.write(frame1)
-        out.write(frame2)
-        out.release()
-        
-        # more pythonic
-        with ffmpegcv.VideoWriter('outpy.mp4', None, 10) as out:
-            out.write(frame1)
-            out.write(frame2)
-        ```
-        
-        
-        Use GPU to accelerate encoding. Such as h264_nvenc, hevc_nvenc.
-        ```python
-        out_cpu = ffmpegcv.VideoWriter('outpy.mp4', None, 10)
-        out_gpu0 = ffmpegcv.VideoWriterNV('outpy.mp4', 'h264', 10)        #NVIDIA GPU0
-        out_gpu1 = ffmpegcv.VideoWriterNV('outpy.mp4', 'hevc', 10, gpu=1) #NVIDIA GPU1
-        ```
-        
-        Input image is rgb24 instead of bgr24
-        ```python
-        out = ffmpegcv.VideoWriter('outpy.mp4', None, 10, pix_fmt='rgb24')
-        out.write(cv2.cvtColor(frame, cv2.COLOR_BGR2RGB))
-        ```
-        
-        ## Video Reader and Writer
-        ---
-        ```python
-        import ffmpegcv
-        vfile_in = 'A.mp4'
-        vfile_out = 'A_h264.mp4'
-        vidin = ffmpegcv.VideoCapture(vfile_in)
-        vidout = ffmpegcv.VideoWriter(vfile_out, None, vidin.fps)
-        
-        with vidin, vidout:
-            for frame in vidin:
-                vidout.write(frame)
-        ```
-        
-        ## Camera Reader
-        ---
-        ***Experimental feature**. The ffmpegcv offers Camera reader. Which is consistent with VideoFiler reader. 
-        
-        - The `VideoCaptureCAM` aims to support ROI operations. The Opencv will be general fascinating than ffmpegcv in camera read. **I recommand the opencv in most camera reading case**.
-        - The ffmpegcv can use name to retrieve the camera device. Use `ffmpegcv.VideoCaptureCAM("Integrated Camera")` is readable than `cv2.VideoCaptureCAM(0)`.
-        - The `VideoCaptureCAM` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
-        - The `VideoCaptureCAM` is continously working on background even if you didn't read it. Please release it in time.
-        - Works perfect in Windows, not-perfect in Linux and macOS.
-        
-        ```python
-        import cv2
-        cap = cv2.VideoCapture(0)
-        while True:
-            ret, frame = cap.read()
-            cv2.imshow('frame', frame)
-            if cv2.waitKey(1) & 0xFF == ord('q'):
-                break
-        cap.release()
-        
-        # ffmpegcv, in Windows&Linux
-        import ffmpegcv
-        cap = ffmpegcv.VideoCaptureCAM(0)
-        while True:
-            ret, frame = cap.read()
-            cv2.imshow('frame', frame)
-            if cv2.waitKey(1) & 0xFF == ord('q'):
-                break
-        cap.release()
-        
-        # ffmpegcv use by camera name, in Windows&Linux
-        cap = ffmpegcv.VideoCaptureCAM("Integrated Camera")
-        
-        # ffmpegcv use camera path if multiple cameras conflict
-        cap = ffmpegcv.VideoCaptureCAM('@device_pnp_\\\\?\\usb#vid_2304&'
-            'pid_oot#media#0001#{65e8773d-8f56-11d0-a3b9-00a0c9223196}'
-            '\\global')
-        
-        # ffmpegcv use camera with ROI operations
-        cap = ffmpegcv.VideoCaptureCAM("Integrated Camera", crop_xywh=(0, 0, 640, 480), resize=(512, 512), resize_keepratio=True)
-        
-        
-        ```
-        
-        **list all camera devices**
-        ```python
-        from ffmpegcv.ffmpeg_reader_camera import query_camera_devices
-        
-        devices = query_camera_devices()
-        print(devices)
-        ```
-        >{0: ('Integrated Camera', '@device_pnp_\\\\?\\usb#vid_2304&pid_oot#media#0001#{65e8773d-8f56-11d0-a3b9-00a0c9223196}\\global'),  
-        1: ('OBS Virtual Camera', '@device_sw_{860BB310-5D01-11D0-BD3B-00A0C911CE86}\\{A3FCE0F5-3493-419F-958A-ABA1250EC20B}')}
-        
-        
-        **Set the camera resolution, fps, vcodec/pixel-format**
-        
-        ```python
-        from ffmpegcv.ffmpeg_reader_camera import query_camera_options
-        
-        options = query_camera_options(0)  # or query_camera_options("Integrated Camera") 
-        print(options)
-        cap = ffmpegcv.VideoCaptureCAM(0, **options[-1])
-        ```
-        >[{'camcodec': 'mjpeg', 'campix_fmt': None, 'camsize_wh': (1280, 720), 'camfps': 60.0002}, {'camcodec': 'mjpeg', 'campix_fmt': None, 'camsize_wh': (640, 480), 'camfps': 60.0002}, {'camcodec': 'mjpeg', 'campix_fmt': None, 'camsize_wh': (1920, 1080), 'camfps': 60.0002}, {'camcodec': None, 'campix_fmt': 'yuyv422', 'camsize_wh': (1280, 720), 'camfps': 10}, {'camcodec': None, 'campix_fmt': 'yuyv422', 'camsize_wh': (640, 480), 'camfps': 30}, {'camcodec': None, 'campix_fmt': 'yuyv422', 'camsize_wh': (1920, 1080), 'camfps': 5}]
-        
-        **Known issues**
-        1. The VideoCaptureCAM didn't give a smooth experience in macOS. You must specify all the camera parameters. And the query_camera_options woun't give any suggestion. That's because the `ffmpeg` cannot list device options using mac native `avfoundation`. 
-        ```python
-        # The macOS requires full argument.
-        cap = ffmpegcv.VideoCaptureCAM('FaceTime HD Camera', camsize_wh=(1280,720), camfps=30, campix_fmt='nv12')
-        ```
-        
-        2. The VideoCaptureCAM cann't list the FPS in linux. Because the `ffmpeg` cound't query the device's FPS using linux native `v4l2` module. However, it's just OK to let the FPS blank.
-        
-Platform: UNKNOWN
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+# FFMPEGCV is an alternative to OPENCV for video read and write.
+The ffmpegcv provide Video Reader and Video Witer with ffmpeg backbone, which are faster and powerful than cv2.
+
+- The ffmpegcv is api **compatible** to open-cv. 
+- The ffmpegcv can use **GPU accelerate** encoding and decoding*. 
+- The ffmpegcv support much more video **codecs** v.s. open-cv.
+- The ffmpegcv support **RGB** & BGR format as you like.
+- The ffmpegcv can support ROI operations.You can **crop**, **resize** and **pad** the ROI.
+
+In all, ffmpegcv is just similar to opencv api. But is faster* and with more codecs.
+
+
+## Basic example
+Read a video by CPU, and rewrite it by GPU.
+```python
+vidin = ffmpegcv.VideoCapture(vfile_in)
+vidout = ffmpegcv.VideoWriterNV(vfile_out, 'h264', vidin.fps)
+
+with vidin, vidout:
+    for frame in vidin:
+        cv2.imshow('image', frame)
+        vidout.write(frame)
+```
+
+Read the camera by device name.
+```python
+cap = ffmpegcv.VideoCaptureCAM("Integrated Camera")
+```
+
+## Install
+You need to download ffmpeg before you can use ffmpegcv
+> conda install ffmpeg 
+>
+> pip install ffmpegcv
+
+## GPU Accelation
+- Support NVIDIA card only.
+- Perfect in the **Windows**. That ffmpeg supports NVIDIA acceleration just by conda install.
+- Struggle in the **Linux**. That ffmpeg didn't orginally support NVIDIA accelerate.
+Please re-compile the ffmpeg by yourself.
+See the [link](https://docs.nvidia.com/video-technologies/video-codec-sdk/ffmpeg-with-nvidia-gpu/)
+- Works in the **Google Colab** notebook without pain (no need to recompile ffmpeg). 
+- Infeasible in the **MacOS**. That ffmpeg didn't supports NVIDIA at all.
+
+> \* The ffmegcv GPU reader is a bit slower than CPU reader, but much faster when use ROI operations (crop, resize, pad).
+
+## Codecs
+
+| Codecs      | OpenCV-reader | ffmpegcv-cpu-r     | gpu-r  | OpenCV-writer | ffmpegcv-cpu-w     | gpu-w  |
+| ----------- | ------------- | ---------------- | ---- | ------------- | ---------------- | ---- |
+| h264        | √             | √                | √    | ×             | √                | √    |
+| h265 (hevc) | not sure      | √                | √    | ×             | √                | √    |
+| mjpeg       | √             | √                | ×    | √             | √                | ×    |
+| mpeg        | √             | √                | ×    | √             | √                | ×    |
+| others      | not sure      | ffmpeg -decoders | ×    | not sure      | ffmpeg -encoders | ×    |
+
+## Benchmark
+*On the way...*
+
+
+## Video Reader
+---
+The ffmpegcv is just similar to opencv in api.
+```python
+# open cv
+import cv2
+cap = cv2.VideoCapture(file)
+while True:
+    ret, frame = cap.read()
+    if not ret:
+        break
+    pass
+
+# ffmpegcv
+import ffmpegcv
+cap = ffmpegcv.VideoCapture(file)
+while True:
+    ret, frame = cap.read()
+    if not ret:
+        break
+    pass
+cap.release()
+
+# alternative
+cap = ffmpegcv.VideoCapture(file)
+nframe = len(cap)
+for frame in cap:
+    pass
+cap.release()
+
+# more pythonic, recommand
+with ffmpegcv.VideoCapture(file) as cap:
+    nframe = len(cap)
+    for iframe, frame in enumerate(cap):
+        if iframe>100: break
+        pass
+```
+
+Use GPU to accelerate decoding. It depends on the video codes.
+h264_nvcuvid, hevc_nvcuvid ....
+```python
+cap_cpu = ffmpegcv.VideoCapture(file)
+cap_gpu = ffmpegcv.VideoCapture(file, codec='h264_cuvid') #NVIDIA GPU0
+cap_gpu0 = ffmpegcv.VideoCaptureNV(file)         #NVIDIA GPU0
+cap_gpu1 = ffmpegcv.VideoCaptureNV(file, gpu=1)  #NVIDIA GPU1
+```
+
+Use rgb24 instead of bgr24
+```python
+cap = ffmpegcv.VideoCapture(file, pix_fmt='rgb24')
+ret, frame = cap.read()
+plt.imshow(frame)
+```
+
+### ROI Operations
+You can crop, resize and pad the video. These ROI operation is `ffmpegcv-GPU` > `ffmpegcv-CPU` >> `opencv`.
+
+**Crop** video, which will be much faster than read the whole canvas.
+```python
+cap = ffmpegcv.VideoCapture(file, crop_xywh=(0, 0, 640, 480))
+```
+
+**Resize** the video to the given size.
+```python
+cap = ffmpegcv.VideoCapture(file, resize=(640, 480))
+```
+
+**Resize** and keep the aspect ratio with black border **padding**.
+```python
+cap = ffmpegcv.VideoCapture(file, resize=(640, 480), resize_keepratio=True)
+```
+
+**Crop** and then **resize** the video.
+```python
+cap = ffmpegcv.VideoCapture(file, crop_xywh=(0, 0, 640, 480), resize=(512, 512))
+```
+
+## Video Writer
+---
+```python
+# cv2
+out = cv2.VideoWriter('outpy.avi',
+                       cv2.VideoWriter_fourcc('M','J','P','G'), 
+                       10, 
+                       (w, h))
+out.write(frame1)
+out.write(frame2)
+out.release()
+
+# ffmpegcv, default codec is 'h264' in cpu 'h265' in gpu.
+# frameSize is decided by the size of the first frame
+out = ffmpegcv.VideoWriter('outpy.mp4', None, 10)
+out.write(frame1)
+out.write(frame2)
+out.release()
+
+# more pythonic
+with ffmpegcv.VideoWriter('outpy.mp4', None, 10) as out:
+    out.write(frame1)
+    out.write(frame2)
+```
+
+
+Use GPU to accelerate encoding. Such as h264_nvenc, hevc_nvenc.
+```python
+out_cpu = ffmpegcv.VideoWriter('outpy.mp4', None, 10)
+out_gpu0 = ffmpegcv.VideoWriterNV('outpy.mp4', 'h264', 10)        #NVIDIA GPU0
+out_gpu1 = ffmpegcv.VideoWriterNV('outpy.mp4', 'hevc', 10, gpu=1) #NVIDIA GPU1
+```
+
+Input image is rgb24 instead of bgr24
+```python
+out = ffmpegcv.VideoWriter('outpy.mp4', None, 10, pix_fmt='rgb24')
+out.write(cv2.cvtColor(frame, cv2.COLOR_BGR2RGB))
+```
+
+## Video Reader and Writer
+---
+```python
+import ffmpegcv
+vfile_in = 'A.mp4'
+vfile_out = 'A_h264.mp4'
+vidin = ffmpegcv.VideoCapture(vfile_in)
+vidout = ffmpegcv.VideoWriter(vfile_out, None, vidin.fps)
+
+with vidin, vidout:
+    for frame in vidin:
+        vidout.write(frame)
+```
+
+## Camera Reader
+---
+**Experimental feature**. The ffmpegcv offers Camera reader. Which is consistent with VideoFiler reader. 
+
+- The `VideoCaptureCAM` aims to support ROI operations. The Opencv will be general fascinating than ffmpegcv in camera read. **I recommand the opencv in most camera reading case**.
+- The ffmpegcv can use name to retrieve the camera device. Use `ffmpegcv.VideoCaptureCAM("Integrated Camera")` is readable than `cv2.VideoCaptureCAM(0)`.
+- The `VideoCaptureCAM` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
+- The `VideoCaptureCAM` is continously working on background even if you didn't read it. Please release it in time.
+- Works perfect in Windows, not-perfect in Linux and macOS.
+
+```python
+import cv2
+cap = cv2.VideoCapture(0)
+while True:
+    ret, frame = cap.read()
+    cv2.imshow('frame', frame)
+    if cv2.waitKey(1) & 0xFF == ord('q'):
+        break
+cap.release()
+
+# ffmpegcv, in Windows&Linux
+import ffmpegcv
+cap = ffmpegcv.VideoCaptureCAM(0)
+while True:
+    ret, frame = cap.read()
+    cv2.imshow('frame', frame)
+    if cv2.waitKey(1) & 0xFF == ord('q'):
+        break
+cap.release()
+
+# ffmpegcv use by camera name, in Windows&Linux
+cap = ffmpegcv.VideoCaptureCAM("Integrated Camera")
+
+# ffmpegcv use camera path if multiple cameras conflict
+cap = ffmpegcv.VideoCaptureCAM('@device_pnp_\\\\?\\usb#vid_2304&'
+    'pid_oot#media#0001#{65e8773d-8f56-11d0-a3b9-00a0c9223196}'
+    '\\global')
+
+# ffmpegcv use camera with ROI operations
+cap = ffmpegcv.VideoCaptureCAM("Integrated Camera", crop_xywh=(0, 0, 640, 480), resize=(512, 512), resize_keepratio=True)
+
+
+```
+
+**list all camera devices**
+```python
+from ffmpegcv.ffmpeg_reader_camera import query_camera_devices
+
+devices = query_camera_devices()
+print(devices)
+```
+>{0: ('Integrated Camera', '@device_pnp_\\\\?\\usb#vid_2304&pid_oot#media#0001#{65e8773d-8f56-11d0-a3b9-00a0c9223196}\\global'),  
+1: ('OBS Virtual Camera', '@device_sw_{860BB310-5D01-11D0-BD3B-00A0C911CE86}\\{A3FCE0F5-3493-419F-958A-ABA1250EC20B}')}
+
+
+**Set the camera resolution, fps, vcodec/pixel-format**
+
+```python
+from ffmpegcv.ffmpeg_reader_camera import query_camera_options
+
+options = query_camera_options(0)  # or query_camera_options("Integrated Camera") 
+print(options)
+cap = ffmpegcv.VideoCaptureCAM(0, **options[-1])
+```
+>[{'camcodec': 'mjpeg', 'campix_fmt': None, 'camsize_wh': (1280, 720), 'camfps': 60.0002}, {'camcodec': 'mjpeg', 'campix_fmt': None, 'camsize_wh': (640, 480), 'camfps': 60.0002}, {'camcodec': 'mjpeg', 'campix_fmt': None, 'camsize_wh': (1920, 1080), 'camfps': 60.0002}, {'camcodec': None, 'campix_fmt': 'yuyv422', 'camsize_wh': (1280, 720), 'camfps': 10}, {'camcodec': None, 'campix_fmt': 'yuyv422', 'camsize_wh': (640, 480), 'camfps': 30}, {'camcodec': None, 'campix_fmt': 'yuyv422', 'camsize_wh': (1920, 1080), 'camfps': 5}]
+
+**Known issues**
+1. The VideoCaptureCAM didn't give a smooth experience in macOS. You must specify all the camera parameters. And the query_camera_options woun't give any suggestion. That's because the `ffmpeg` cannot list device options using mac native `avfoundation`. 
+```python
+# The macOS requires full argument.
+cap = ffmpegcv.VideoCaptureCAM('FaceTime HD Camera', camsize_wh=(1280,720), camfps=30, campix_fmt='nv12')
+```
+
+2. The VideoCaptureCAM cann't list the FPS in linux. Because the `ffmpeg` cound't query the device's FPS using linux native `v4l2` module. However, it's just OK to let the FPS blank.
+
+
+## Stream Reader
+**Experimental feature**. The ffmpegcv offers Camera reader. Which is consistent with VideoFiler reader. The feature is like a camera.
+Becareful when using it.
+
+- Support `RTSP`, `RTP`, `RTMP`, `HTTP`, `HTTPS` streams.
+- The `VideoCaptureStream` will be laggy and dropping frames if your post-process takes long time. The VideoCaptureCAM will buffer the recent frames.
+- The `VideoCaptureStream` is continously working on background even if you didn't read it. Please release it in time.
+
+
+```python
+import cv2
+stream_url = 'http://devimages.apple.com.edgekey.net/streaming/examples/bipbop_4x3/gear2/prog_index.m3u8'
+cap = cv2.VideoCapture(stream_url, cv2.CAP_FFMPEG)
+
+if not cap.isOpened():
+    print('Cannot open the stream')
+    exit(-1)
+
+while True:
+    ret, frame = cap.read()
+    if not ret:
+        break
+    pass
+
+# ffmpegcv, in Windows&Linux
+import ffmpegcv
+cap = ffmpegcv.VideoCaptureStream(stream_url)
+while True:
+    ret, frame = cap.read()
+    if not ret:
+        break
+    pass
+```
```

