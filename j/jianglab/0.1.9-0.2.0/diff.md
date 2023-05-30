# Comparing `tmp/jianglab-0.1.9.tar.gz` & `tmp/jianglab-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.1.9.tar", last modified: Mon Apr 24 20:59:30 2023, max compression
+gzip compressed data, was "jianglab-0.2.0.tar", last modified: Tue May 30 15:05:25 2023, max compression
```

## Comparing `jianglab-0.1.9.tar` & `jianglab-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 20:59:30.277179 jianglab-0.1.9/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-24 20:59:30.276857 jianglab-0.1.9/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.1.9/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 20:59:30.273716 jianglab-0.1.9/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       54 2023-04-13 12:28:44.000000 jianglab-0.1.9/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)     9281 2023-04-24 20:56:16.000000 jianglab-0.1.9/jianglab/common_functions.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-04-24 20:59:30.276328 jianglab-0.1.9/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-04-24 20:59:30.000000 jianglab-0.1.9/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      227 2023-04-24 20:59:30.000000 jianglab-0.1.9/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-04-24 20:59:30.000000 jianglab-0.1.9/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       58 2023-04-24 20:59:30.000000 jianglab-0.1.9/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-04-24 20:59:30.000000 jianglab-0.1.9/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-04-24 20:59:30.277293 jianglab-0.1.9/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      830 2023-04-24 20:59:14.000000 jianglab-0.1.9/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:05:25.474161 jianglab-0.2.0/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-05-30 15:05:25.473878 jianglab-0.2.0/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.2.0/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:05:25.470936 jianglab-0.2.0/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       54 2023-04-13 12:28:44.000000 jianglab-0.2.0/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    12499 2023-05-30 15:04:44.000000 jianglab-0.2.0/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:03:09.000000 jianglab-0.2.0/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-05-30 15:05:25.473360 jianglab-0.2.0/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      542 2023-05-30 15:05:25.000000 jianglab-0.2.0/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-05-30 15:05:25.000000 jianglab-0.2.0/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-05-30 15:05:25.000000 jianglab-0.2.0/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       93 2023-05-30 15:05:25.000000 jianglab-0.2.0/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-05-30 15:05:25.000000 jianglab-0.2.0/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-05-30 15:05:25.474279 jianglab-0.2.0/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      909 2023-05-30 15:04:43.000000 jianglab-0.2.0/setup.py
```

### Comparing `jianglab-0.1.9/README.md` & `jianglab-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.1.9/jianglab/common_functions.py` & `jianglab-0.2.0/jianglab/common_functions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 import os
 from treelib import Tree, Node 
 import numpy as np
 import McsPy.McsCMOSMEA as McsCMOSMEA
 from tqdm import tqdm
 from scipy.signal import find_peaks
 import matplotlib.pyplot as plt
+import gspread
+import pandas as pd
+from oauth2client.service_account import ServiceAccountCredentials
+import scipy.signal as signal
+import pickle
+import os
 
 def frame_ref_to_onset(frame_ref, first_onset_index = 184, visualize_window = (250_000,350_000), stimulus_interval = 60, on_duration = 30, sampling_rate = 20000,overlay_split_num = 5):
-    plt.rcParams['figure.figsize'] = [30, 5]
-    def frame_ref_to_onset_plot(frame_ref = frame_ref, first_onset_index = first_onset_index, stimulus_interval = stimulus_interval, on_duration = on_duration, sampling_rate = sampling_rate, overlay_split_num = overlay_split_num, find_first_onset = True, visualize_window = visualize_window):
-        '''
+    '''
         Convert frame_ref to onset_index
         input:
             frame_ref: 2d array, first row is the light, second row is the frame
             first_onset_index: the index of the first onset, it needs to be manually adjusted
             stimulus_interval: the interval between two stimulus in a unit of frame number
             sampling_rate: the sampling rate of the frame_ref
         output:
             It plots the frame_ref and the onset_index with index number
         return: 
             onset_index: the index of all onsets in a unit of sampling number according to sampling_rate
             off_set_index: the index of all offsets in a unit of sampling number according to sampling_rate
             peaks: the index of all frames in a unit of sampling number according to sampling_rate
             first_onset_index: the index of the first onset
         '''
+    plt.rcParams['figure.figsize'] = [30, 5]
+    def frame_ref_to_onset_plot(frame_ref = frame_ref, first_onset_index = first_onset_index, stimulus_interval = stimulus_interval, on_duration = on_duration, sampling_rate = sampling_rate, overlay_split_num = overlay_split_num, find_first_onset = True, visualize_window = visualize_window):
+        
         prominence = 0.5 * max(frame_ref[1])
         distance = sampling_rate / (stimulus_interval + 10)
         peaks, _ = find_peaks(frame_ref[1], prominence=prominence,distance=distance)
         onset_index = peaks[first_onset_index:][::stimulus_interval] # the index of all onsets in a unit of sampling number according to sampling_rate
         offset_index = peaks[first_onset_index + on_duration:][::stimulus_interval]
         
         # lable the peaks with index number
@@ -189,10 +196,82 @@
         tree.create_node(tag=tag, identifier=node_id, parent=parent_id)
         
         if isinstance(value, dict):
             dict_to_tree(value, parent_id=node_id, tree=tree)
 
     return tree
 
+def import_gsheet(sheet_name = params.sheet_name,
+                cred = params.google_cred
+                ):
+
+    for i in range(3):# search parent folder
+        if not os.path.exists(cred): 
+            cred = "." + cred
+
+    scope = params.scope
+    creds_obj = ServiceAccountCredentials.from_json_keyfile_name(cred, scope)
+    client = gspread.authorize(creds_obj)
+    sheet = client.open(sheet_name).sheet1.get_all_records()
+    df = pd.DataFrame.from_dict(sheet)
+    df.to_csv("../gsheet_table.csv", index = False)
+    return df
+
+def resample_med(np_array, kernel_size = 100, resample_rate =10): # med filter through first axis
+    counter = 0
+    out_array = np.zeros_like(np_array)
+    for i in range(np_array.shape[1]):
+        for j in range(np_array.shape[2]):
+            counter += 1
+            if counter % 100 == 0:
+                print(counter, " out of 4225")
+            out_array[:,i,j] = signal.medfilt(np_array[:,i,j], kernel_size=kernel_size)
+    return out_array[::resample_rate]
+
+
+def remove_bad_lanes(data, bad_lanes): # for low pass filtered data
+    data = np.delete(data, [int(lane)-1 for lane in bad_lanes], axis= 2)
+    return data
+
+def save_instance(filename, instance):
+    with open(filename, "wb") as file_:
+        pickle.dump(instance, file_, -1)
+
+def load_instance(filename):
+    return pickle.load(open(filename, "rb", -1))
+
+def find_3d_local_min_general(arr, neighbor_size =  params.center_search_range):
+    if arr.shape[0] != 0:
+        counter = 0
+        neighbor_size = np.array(neighbor_size)
+        pad =  (neighbor_size/2).astype(np.int)
+        arr_pad = np.pad(arr, ((pad[0],pad[0]), (pad[1],pad[1]), (pad[2],pad[2])), 'constant', constant_values = arr.max())
+        arr_pad = arr_pad.astype(np.int)
+        center_list = []
+        i_range, j_range, k_range = (arr_pad.shape[0]-pad[0]),(arr_pad.shape[1]-pad[1]),(arr_pad.shape[2]-pad[2])
+        #surround_varience = []
+        for i in tqdm(range(0, i_range,1), desc="Roughly find 3d local minimal"):
+            for j in range(j_range):
+                for k in range(k_range):
+                    m,n,p = neighbor_size
+                    try:
+                        if i >= pad[0] and j >= pad[1] and k >= pad[2]:
+                            surround = arr_pad[i+pad[0]-m:i+pad[0]+m,j+pad[1]-n:j+pad[1]+n,k+pad[2]-p:k+pad[2]+p]
+                            surround[m, n, p] = surround[m, n, p]+1
+                            if np.all(arr_pad[i,j,k] <= surround):
+                                center_list.append([i-pad[0],j-pad[1],k-pad[2]])
+                                counter+=1
+                                # if counter % 100 ==0:
+                                #     print(i-pad[0],j-pad[1],k-pad[2])
+                                #     print(counter)
+                            else:
+                                pass
+                    except OSError as e:
+                        print(e)
+        return np.array(center_list)
+    else:
+        print("Empty input. Detection failed.")
+        return np.array([0,0,0])
+    
 
 def func3():
     pass
```

### Comparing `jianglab-0.1.9/setup.py` & `jianglab-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.1.9',
+    version='0.2.0',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
         "tqdm",
         "scipy",
+        "gspread",
+        "oauth2client",
+        "parmas",
+        "pickle"
+
     ],
     author = "Jiang Zheng",
     author_email = "zjiang314@gmail.com",
     description = "A package for Jiang lab",
     url = "https://github.com/jiang-lab-retina/jianglab.git",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

