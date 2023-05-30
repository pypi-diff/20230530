# Comparing `tmp/streamlitopencvplayer-1.2.0.tar.gz` & `tmp/streamlitopencvplayer-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.2.0.tar", last modified: Mon May 29 13:26:48 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.2.1.tar", last modified: Tue May 30 10:39:08 2023, max compression
```

## Comparing `streamlitopencvplayer-1.2.0.tar` & `streamlitopencvplayer-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 13:26:48.883677 streamlitopencvplayer-1.2.0/
--rw-rw-rw-   0        0        0      419 2023-05-29 13:26:48.882677 streamlitopencvplayer-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-29 13:26:48.884676 streamlitopencvplayer-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-05-29 13:26:28.000000 streamlitopencvplayer-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 13:26:48.850693 streamlitopencvplayer-1.2.0/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.2.0/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     7668 2023-05-29 13:11:21.000000 streamlitopencvplayer-1.2.0/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-05-29 13:26:48.869680 streamlitopencvplayer-1.2.0/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-05-29 13:26:48.000000 streamlitopencvplayer-1.2.0/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-05-29 13:26:48.000000 streamlitopencvplayer-1.2.0/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 13:26:48.000000 streamlitopencvplayer-1.2.0/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-29 13:26:48.000000 streamlitopencvplayer-1.2.0/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 13:26:48.877680 streamlitopencvplayer-1.2.0/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.2.0/test/__init__.py
--rw-rw-rw-   0        0        0      818 2023-05-25 21:34:02.000000 streamlitopencvplayer-1.2.0/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:39:08.400972 streamlitopencvplayer-1.2.1/
+-rw-rw-rw-   0        0        0      419 2023-05-30 10:39:08.398974 streamlitopencvplayer-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-30 10:39:08.401973 streamlitopencvplayer-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-05-30 10:38:59.000000 streamlitopencvplayer-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:39:08.369844 streamlitopencvplayer-1.2.1/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.2.1/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     6852 2023-05-30 10:35:27.000000 streamlitopencvplayer-1.2.1/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:39:08.387922 streamlitopencvplayer-1.2.1/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-05-30 10:39:08.000000 streamlitopencvplayer-1.2.1/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-05-30 10:39:08.000000 streamlitopencvplayer-1.2.1/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 10:39:08.000000 streamlitopencvplayer-1.2.1/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-30 10:39:08.000000 streamlitopencvplayer-1.2.1/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 10:39:08.395136 streamlitopencvplayer-1.2.1/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.2.1/test/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-05-30 09:40:55.000000 streamlitopencvplayer-1.2.1/test/test.py
```

### Comparing `streamlitopencvplayer-1.2.0/README.md` & `streamlitopencvplayer-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.2.0/setup.py` & `streamlitopencvplayer-1.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2.0' 
+VERSION = '1.2.1' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.2.0/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.2.1/streamlitopencvplayer/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,87 +101,72 @@
     # back to the first frame if the video is finished
     if st.session_state['counter'] == len(st.session_state['frames']):
         st.session_state['counter'] = 0
         if 'myslider' in st.session_state:
             del st.session_state.myslider
     stframe.image(st.session_state['frames']
                   [st.session_state['counter']], caption='', width=450)
-    try:
-        while st.session_state['counter'] < len(st.session_state['frames']):
-            if not resume:
-                if i < len(data):
-                    if st.session_state['counter'] == int(alerts[i]*fps):
-                        # draw all detections on the frame
-                        for j in range(len(data[i])):
-                            output = cv2.rectangle(st.session_state['frames'][st.session_state['counter']], (data[i][j][0][0], data[i][j][0][1]), (
-                                data[i][j][0][2], data[i][j][0][3]), color=(128, 0, 0), thickness=2)
-                            output = cv2.putText(
-                                st.session_state['frames'][st.session_state['counter']], data[i][j][3], (data[i][j][0][0], data[i][j][0][1]-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 0, 255), 2)
-                        # update image zone with detections
-                        stframe.image(output, caption='', width=500)
-                        time.sleep(0.08)
-                        # the detection is drawn, to the next one
-                        i += 1
-                        st.session_state['counter'] += 1
-                        # frame_number.slider_changed(st.session_state['counter'])
-
-                        # update slider value
-                        widget.slider("", min_value=0, max_value=int(
-                            cap.get(cv2.CAP_PROP_FRAME_COUNT)), value=st.session_state['counter'], on_change=display_value)
-                stframe.image(
-                    st.session_state['frames'][st.session_state['counter']], caption='', width=500)
-                time.sleep(0.08)
-                st.session_state['counter'] += 1
-                # update slider value
-
-                frame_num = widget.slider("", min_value=0, max_value=int(
-                    cap.get(cv2.CAP_PROP_FRAME_COUNT)), value=st.session_state['counter'], on_change=display_value)
-                if 'myslider' in st.session_state:
-                    if st.session_state.myslider > frame_num:
-                        del st.session_state.myslider
-                        #st.session_state.clear()
-                        st.session_state['counter'] = frame_num
-                        #st.session_state['counter'] = 0
-                        resume = True
-                        #st.experimental_rerun() #remove cache
-                    
 
-                if pause:
+    while st.session_state['counter'] < len(st.session_state['frames']):
+        if not resume:
+            if i < len(data):
+                if st.session_state['counter'] == int(alerts[i]*fps):
+                    # draw all detections on the frame
+                    for j in range(len(data[i])):
+                        output = cv2.rectangle(st.session_state['frames'][st.session_state['counter']], (data[i][j][0][0], data[i][j][0][1]), (
+                            data[i][j][0][2], data[i][j][0][3]), color=(128, 0, 0), thickness=2)
+                        output = cv2.putText(
+                            st.session_state['frames'][st.session_state['counter']], data[i][j][3], (data[i][j][0][0], data[i][j][0][1]-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 0, 255), 2)
+                    # update image zone with detections
+                    stframe.image(output, caption='', width=500)
+                    time.sleep(0.08)
+                    # the detection is drawn, to the next one
+                    i += 1
+                    st.session_state['counter'] += 1
+                    # frame_number.slider_changed(st.session_state['counter'])
+
+                    # update slider value
+                    widget.slider("", min_value=0, max_value=int(
+                        cap.get(cv2.CAP_PROP_FRAME_COUNT)), value=st.session_state['counter'], on_change=display_value)
+            stframe.image(
+                st.session_state['frames'][st.session_state['counter']], caption='', width=500)
+            time.sleep(0.08)
+            st.session_state['counter'] += 1
+            # update slider value
+
+            frame_num = widget.slider("", min_value=0, max_value=int(
+                cap.get(cv2.CAP_PROP_FRAME_COUNT)), value=st.session_state['counter'], on_change=display_value)
+            if 'myslider' in st.session_state:
+                if st.session_state.myslider > frame_num:
+                    del st.session_state.myslider
+                    #st.session_state.clear()
+                    st.session_state['counter'] = frame_num
+                    #st.session_state['counter'] = 0
                     resume = True
-                    break
-                if plus:
-                    resume = True
-                    break
-                if minus:
-                    st.session_state['counter'] -= 1
-                    resume = True
-                    break
-                if replay:
-                    st.session_state['counter'] = 0
-                    st.session_state['frames'] = []
-                    # back to the first frame if the video is finished
-                if st.session_state['counter'] == len(st.session_state['frames']):
-                    st.session_state['counter'] = 0
-                    if 'myslider'  in st.session_state:
-                        del st.session_state.myslider
-                st.session_state['counter'] = frame_num
-    except Exception as e:
-        st.write('')
+                    #st.experimental_rerun() #remove cache
+                
+
+            if pause:
+                resume = True
+                break
+            if plus:
+                resume = True
+                break
+            if minus:
+                st.session_state['counter'] -= 1
+                resume = True
+                break
+            if replay:
+                st.session_state['counter'] = 0
+                st.session_state['frames'] = []
+                # back to the first frame if the video is finished
+            if st.session_state['counter'] == len(st.session_state['frames']):
+                st.session_state['counter'] = 0
+                if 'myslider'  in st.session_state:
+                    del st.session_state.myslider
+            st.session_state['counter'] = frame_num
+
     if resume:
         container_2.empty()
         pause = container_2.button('▶')
         resume = False
 
-
-def main():
-
-    my_dict = {"Alerts": [43, 64]}
-    alerts = [43, 64]
-    data = [[[10, 100, 290, 200], 0.82, 0, "Class 0"],
-            [[55, 22, 100, 120], 0.9, 1, "Class 1"]]
-    video_path = "https://cvlogger.blob.core.windows.net/clientsample/1678352121.8713963_1678352127.8713963.webm?se=2023-05-29T14%3A09%3A37Z&sp=r&sv=2021-08-06&sr=b&sig=y2dF5a%2BUN7inLzOHJgOLmECl7h9iOHFH5dP8BsIF9Bc%3D"
-    if video_path is not None:
-        display_video(video_path, my_dict, alerts, data)
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `streamlitopencvplayer-1.2.0/test/test.py` & `streamlitopencvplayer-1.2.1/test/test.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,18 +7,19 @@
     st.session_state['counter'] = 0
 if 'frames' not in st.session_state:
     st.session_state['frames'] = []
 
 
 def main():
 
-    alerts_dict = {"Alerts": [43, 64]}
+    my_dict = {"Alerts": [43, 64]}
     alerts = [43, 64]
     data = [[[10, 100, 290, 200], 0.82, 0, "Class 0"],
             [[55, 22, 100, 120], 0.9, 1, "Class 1"]]
-    video_path = "https://cvlogger.blob.core.windows.net/clientsample/1678352121.8713963_1678352127.8713963.webm?se=2023-05-25T14%3A31%3A49Z&sp=r&sv=2021-08-06&sr=b&sig=358A3taHXFqd86m7CRCk9tbGW6V5K73nBD8H%2Bsu9QWk%3D"
+    video_path = "https://cvlogger.blob.core.windows.net/clientsample/1678352121.8713963_1678352127.8713963.webm?se=2023-05-30T10%3A40%3A30Z&sp=r&sv=2021-08-06&sr=b&sig=FwjgwVHcS9Rhb982FjRAyKgyw4bQai7rDHXvdOetK5Y%3D"
     if video_path is not None:
-        display_video(video_path, alerts_dict, alerts, data)
+        display_video(video_path, my_dict, alerts, data)
 
 
 if __name__ == "__main__":
     main()
+
```

