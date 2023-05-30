# Comparing `tmp/opyf-1.3.tar.gz` & `tmp/opyf-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opyf-1.3.tar", last modified: Fri Jan  1 21:29:15 2021, max compression
+gzip compressed data, was "opyf-1.4.tar", last modified: Tue May 30 14:45:22 2023, max compression
```

## Comparing `opyf-1.3.tar` & `opyf-1.4.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-01-01 21:29:15.000000 opyf-1.3/
--rwxrwxrwx   0 root         (0) root         (0)     9163 2021-01-01 21:29:15.000000 opyf-1.3/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-01-01 21:29:15.000000 opyf-1.3/opyf/
--rwxrwxrwx   0 root         (0) root         (0)    67872 2021-01-01 21:22:55.000000 opyf-1.3/opyf/Analyzer.py
--rwxrwxrwx   0 root         (0) root         (0)    15512 2020-04-26 10:03:50.000000 opyf-1.3/opyf/Files.py
--rwxrwxrwx   0 root         (0) root         (0)    12465 2020-04-28 08:30:19.000000 opyf-1.3/opyf/Filters.py
--rwxrwxrwx   0 root         (0) root         (0)     9066 2020-12-31 16:35:22.000000 opyf-1.3/opyf/Interpolate.py
--rwxrwxrwx   0 root         (0) root         (0)      905 2019-12-22 12:21:55.000000 opyf-1.3/opyf/MeshesAndTime.py
--rwxrwxrwx   0 root         (0) root         (0)    46822 2020-05-14 11:29:17.000000 opyf-1.3/opyf/Render.py
--rwxrwxrwx   0 root         (0) root         (0)      489 2020-04-27 10:04:17.000000 opyf-1.3/opyf/Tools.py
--rwxrwxrwx   0 root         (0) root         (0)     5249 2021-01-01 21:07:24.000000 opyf-1.3/opyf/Track.py
--rwxrwxrwx   0 root         (0) root         (0)      414 2019-12-22 12:21:55.000000 opyf-1.3/opyf/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10754 2020-04-26 11:04:47.000000 opyf-1.3/opyf/custom_cmap.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-01-01 21:29:15.000000 opyf-1.3/opyf.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     9163 2021-01-01 21:29:15.000000 opyf-1.3/opyf.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      316 2021-01-01 21:29:15.000000 opyf-1.3/opyf.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2021-01-01 21:29:15.000000 opyf-1.3/opyf.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       60 2021-01-01 21:29:15.000000 opyf-1.3/opyf.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2021-01-01 21:29:15.000000 opyf-1.3/opyf.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2021-01-01 21:29:15.000000 opyf-1.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1728 2021-01-01 21:25:28.000000 opyf-1.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 14:45:22.632613 opyf-1.4/
+-rwxrwxrwx   0 root         (0) root         (0)    35147 2019-12-22 12:21:55.000000 opyf-1.4/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     6770 2023-05-30 14:45:22.632319 opyf-1.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     6092 2023-05-30 11:34:32.000000 opyf-1.4/ReadMe.md
+-rwxrwxrwx   0 root         (0) root         (0)     1057 2023-05-30 14:44:56.000000 opyf-1.4/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-30 14:45:22.632722 opyf-1.4/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 14:45:22.626318 opyf-1.4/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 14:45:22.630602 opyf-1.4/src/opyf/
+-rwxrwxrwx   0 root         (0) root         (0)    63094 2023-05-30 12:24:05.000000 opyf-1.4/src/opyf/Analyzer.py
+-rwxrwxrwx   0 root         (0) root         (0)    15512 2020-04-26 10:03:50.000000 opyf-1.4/src/opyf/Files.py
+-rwxrwxrwx   0 root         (0) root         (0)    13864 2021-10-28 09:42:29.000000 opyf-1.4/src/opyf/Filters.py
+-rwxrwxrwx   0 root         (0) root         (0)     9066 2020-12-31 16:35:22.000000 opyf-1.4/src/opyf/Interpolate.py
+-rwxrwxrwx   0 root         (0) root         (0)      964 2021-05-11 20:04:41.000000 opyf-1.4/src/opyf/MeshesAndTime.py
+-rwxrwxrwx   0 root         (0) root         (0)    47271 2023-05-30 09:56:48.000000 opyf-1.4/src/opyf/Render.py
+-rwxrwxrwx   0 root         (0) root         (0)      489 2020-04-27 10:04:17.000000 opyf-1.4/src/opyf/Tools.py
+-rwxrwxrwx   0 root         (0) root         (0)     5239 2022-05-16 12:26:51.000000 opyf-1.4/src/opyf/Track.py
+-rwxrwxrwx   0 root         (0) root         (0)      414 2019-12-22 12:21:55.000000 opyf-1.4/src/opyf/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10754 2021-03-08 14:14:06.000000 opyf-1.4/src/opyf/custom_cmap.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-30 14:45:22.631947 opyf-1.4/src/opyf.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     6770 2023-05-30 14:45:22.000000 opyf-1.4/src/opyf.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      400 2023-05-30 14:45:22.000000 opyf-1.4/src/opyf.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-30 14:45:22.000000 opyf-1.4/src/opyf.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      105 2023-05-30 14:45:22.000000 opyf-1.4/src/opyf.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-05-30 14:45:22.000000 opyf-1.4/src/opyf.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `opyf-1.3/opyf/Analyzer.py` & `opyf-1.4/src/opyf/Analyzer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Wed Jul 10 08:59:41 2019
 
 @author: Gauthier ROUSSEAU
 """
-
+#%%
 import os
 import sys
 import numpy as np
 import cv2
 from opyf import MeshesAndTime, Track, Render, Files, Tools, Interpolate, Filters
 import matplotlib.pyplot as plt
 import time
 import opyf
 import matplotlib as mpl
 import re
-
+#%%
 
 class Analyzer():
     def __init__(
             self,
             imageROI=None,
             num='opyfPlot',
             mute=False,
@@ -40,16 +40,18 @@
         self.listD = listD
         self.folder_src = folder_src
         self.frameInit = frameInit
         self.number_of_frames = number_of_frames
         print('Dimensions :\n \t', 'Width :',
               self.frameInit.shape[1], 'Height :', self.frameInit.shape[0])
         self.num = num
-        self.mute = mute
         self.display = display
+        self.mute = mute
+        if self.display is False:
+            self.mute = True
         self.scaled = False
         self.scale = 1
         if imageROI is None:
             self.ROI = [0, 0, self.frameInit.shape[1], self.frameInit.shape[0]]
         else:
             self.ROI = imageROI
         print('Regio Of Interest :\n \t', self.ROI)
@@ -75,23 +77,19 @@
 #        self.Xsamples = []
 
         self.unit = args.get('unit', ['px', 'deltaT'])
 
         self.set_imageParams(**args)
         self.paramPlot = {
             'ScaleVectors': args.get(
-                'ScaleVectors', 0.1), 'vecX': [], 'vecY': [], 'extentFrame': args.get(
-                'extentFrame', [
-                    0, self.Lvis, self.Hvis, 0]), 'unit': args.get(
-                    'unit', [
-                        'px', 'deltaT']), 'Hfig': args.get(
-                            'Hfig', 8), 'grid': args.get(
-                                'grid', True), 'vlim': args.get(
-                                    'vlim', [
-                                        0, 40])}
+            'ScaleVectors', 0.1), 'vecX': [], 'vecY': [], 
+            'extentFrame': args.get('extentFrame', [0, self.Lvis, self.Hvis, 0]), 
+            'unit': args.get('unit', ['px', 'deltaT']), 'Hfig': args.get('Hfig', 8),
+            'force_figsize': args.get('force_figsize', None),'grid': args.get( 'grid', True), 
+            'vlim': args.get('vlim', [ 0, 40])}
         self.birdEyeMod = False
         self.stabilizeOn = False
 
         self.close_at_reset = close_at_reset
         self.reset(first=True)
         self.set_gridToInterpolateOn()
 
@@ -196,30 +194,29 @@
 
         print('')
         print('Filters Params:')
         for x in self.filters_params:
             print('\t- ', x, ':', self.filters_params[x])
 
     # When the data set is scaled the radius must be gven in the good length
-    # unity (meter, cm, ....)
+    # unity (meter, cm, ....) 
     def set_interpolationParams(
             self,
             Radius=None,
-            Sharpness=8,
+            Sharpness=8,  
             kernel='Gaussian'):
         if Radius is None:
             Radius = self.scale * 30  # 30 px when the data set is not scaled
-            self.interp_params = dict(Radius=Radius,  
-                                      Sharpness=Sharpness,
-                                      kernel=kernel)
         else:
             Radius = Radius
     # set the a scaled value if the user does not introduce a Radius and the
     # data set is scaled
-
+        self.interp_params = dict(Radius=Radius,  
+                                      Sharpness=Sharpness,
+                                      kernel=kernel)
         print('')
         print('Interpolation Parameters:')
         for x in self.interp_params:
             print('\t- ', x, ':', self.interp_params[x])
 
     def set_vlim(self, vlim):
         if not self.scaled:
@@ -248,28 +245,27 @@
             stepGrid=None):
         if pixRight == 0:
             pixRight = self.Lvis
         if pixDown == 0:
             pixDown = self.Hvis
         if stepGrid is not None:
             stepVert, stepHor = stepGrid, stepGrid
+
         if ROI is not None:
             self.ROImeasure = ROI
             pixLeft, pixRight, pixUp, pixDown = ROI[0], ROI[0] + \
                 ROI[2], ROI[1], ROI[1] + ROI[3]
         else:
             self.ROImeasure = [
                 pixLeft,
                 pixUp,
                 pixRight - pixLeft,
                 pixDown - pixUp]
         self.grid_y, self.grid_x, self.gridVx, self.gridVy, self.Hgrid, self.Lgrid = MeshesAndTime.set_gridToInterpolateOn(
             pixLeft, pixRight, stepHor, pixUp, pixDown, stepVert)
-        self.grid_x = self.grid_x
-        self.grid_y = self.grid_y
 
         if self.scaled:
             self.grid_y, self.grid_x = - \
                 (self.grid_y - self.origin[1]) * \
                 self.scale, (self.grid_x - self.origin[0]) * self.scale
 
         self.vecX = self.grid_x[0, :]
@@ -376,19 +372,19 @@
                               'detect_interval': detection_interval}
 
         self.paramVecTimeTracks = {'starting_frame': starting_frame,
                                    'step': step,
                                    'Ntot': Ntot}
 
         self.vecTracks, self.prevTracks = MeshesAndTime.set_vecTimeTracks(
-            starting_frame=starting_frame, step=step, Ntot=Ntot)
+            starting_frame=starting_frame, step=step,  Ntot=Ntot)
 
         print(
             '\nTracking processing \nTracking operates only in succesives images sperated with [step] frames')
-        if self.vec[-1] > self.number_of_frames:
+        if self.vecTracks[-1] > self.number_of_frames:
             print('----- Error ----')
             print('Your tracking plan is not compatible with the frame set')
             print(
                 'Consider that for tracking [starting_frame+step*(Ntot)]  must be smaller than the number of frames')
             sys.exit()
 
         print('Starting frame : [' + str(starting_frame) + ']')
@@ -414,15 +410,15 @@
             k = 0
             while k < len(self.sortedVec):
                 indF = int(self.cap.get(cv2.CAP_PROP_POS_FRAMES))
                 ret, vis = self.cap.read()
                 if indF == self.sortedVec[k]:
                     self.dictFrames[str(self.sortedVec[k])] = vis
                     k += 1
-        self.readFrame(self.vec[0])
+        self.readFrame(self.vecTracks[0])
 
     def initializeAveragedFrameFromFile(self, file, imreadOption=1):
         frameav = cv2.imread(file, imreadOption)
         frameav = Tools.convertToGrayScale(frameav)
         if frameav is None:
             print('Invalid path for the averaged frame')
         elif frameav.shape != (self.Hvis, self.Lvis):
@@ -514,48 +510,38 @@
 
     def stepTracks(self, pr, i):
         if not pr:
             self.prev_gray = None
         self.currentFrame = i
         self.readFrame(self.currentFrame)
         self.substractAveragedFrame()
-        self.tracks, self.vtracks, self.prev_gray, self.X, self.V = Track.opyfTrack(self.tracks, self.vtracks, self.gray, self.prev_gray,
-                                                                                    self.incr, self.feature_params,
-                                                                                    self.lk_params, self.tracks_params,
-                                                                                    ROI=self.ROImeasure,
-                                                                                    vmin=self.vlimPx[0],
-                                                                                    vmax=self.vlimPx[1],
-                                                                                    mask=self.mask,
-                                                                                    wayBackGoodFlag=self.filters_params['wayBackGoodFlag'])
-
+        self.tracks, self.vtracks, self.prev_gray, self.X, self.V = Track.opyfTrack(self.tracks, self.vtracks, self.gray, self.prev_gray, self.incr, self.feature_params, self.lk_params, self.tracks_params, ROI=self.ROImeasure, vmin=self.vlimPx[0], vmax=self.vlimPx[1], mask=self.mask, wayBackGoodFlag=self.filters_params['wayBackGoodFlag'])
         self.scaleAndLogTracks(i)
 
     def extractTracks(
             self,
             display=False,
             saveImgPath=None,
             numberingOutput=False,
             imgFormat='png',
             **args):
         self.reset()
         self.tracks = []
         self.vtracks = []
         if self.prevTracks is None:
-            print(
-                '\n \nWARNING : To run the extractTracks() method, it is mandatory to define the tracking plan through the method [set_trackingFeatures()]\n\n')
+            print( '\n \nWARNING : To run the extractTracks() method, it is mandatory to define the tracking plan through the method [set_trackingFeatures()]\n\n')
             sys.exit()
         k = 0
         for pr, i in zip(self.prevTracks, self.vecTracks):
             self.stepTracks(pr, i)
             if pr:
                 self.Xdata.append(self.X)
                 self.Vdata.append(self.V)
 
-                cv2.polylines(self.vis, [np.int32(tr)
-                                         for tr in self.tracks], False, (0, 255, 0))
+                cv2.polylines(self.vis, [np.int32(tr) for tr in self.tracks], False, (0, 255, 0))
                 self.showXV(self.X, self.V, vis=self.vis,
                             display=display, **args)
                 if saveImgPath is not None and self.display:
                     if numberingOutput:
                         self.opyfDisp.fig.savefig(
                             str(saveImgPath + '/' + display + '_' + format(k, '04.0f') + '.' + imgFormat))
                         k += 1
@@ -580,32 +566,22 @@
         if not pr:
             self.prev_gray = None
         self.readFrame(i)
         self.substractAveragedFrame()
 
         if self.filters_params['CLAHE']:
             self.gray = Render.CLAHEbrightness(
-                self.gray,
-                0,
+                self.gray, 0,
                 tileGridSize=self.filters_params['gridSize'],
                 clipLimit=self.filters_params['clplim'])
 #             self.vis=Render.CLAHEbrightness(self.vis,0,tileGridSize=(20,20),clipLimit=2)
 
-        self.prev_gray, self.X, self.V = Track.opyfFlowGoodFlag(self.gray,
-                                                                self.prev_gray,
-                                                                self.feature_params,
-                                                                self.lk_params,
-                                                                ROI=self.ROImeasure,
-                                                                vmin=self.vlimPx[0],
-                                                                vmax=self.vlimPx[1],
-                                                                mask=self.mask,
-                                                                wayBackGoodFlag=self.filters_params['wayBackGoodFlag'])
+        self.prev_gray, self.X, self.V = Track.opyfFlowGoodFlag(self.gray, self.prev_gray, self.feature_params, self.lk_params, ROI=self.ROImeasure, vmin=self.vlimPx[0],  vmax=self.vlimPx[1], mask=self.mask, wayBackGoodFlag=self.filters_params['wayBackGoodFlag'])
 
         if pr:
-
             # filters ######
             self.scaleAndLogFlow(i)
             self.X, self.V = self.applyFilters(self.X, self.V)
 
     def applyFilters(self, X, V):
         if self.filters_params['minNperRadius'] > 0:
             print('[I] Number of point within radius (in px) filter')
@@ -657,59 +633,39 @@
             self.V[:, 1] = -self.V[:, 1]
         print('')
         self.incr += 1
         print('-------------- [Tracking - Step ' + str(self.incr) + ' / ' +
               str(self.paramVecTimeTracks['Ntot']) + '] --------------')
 
         if self.processingMode == 'image sequence':
-            print('------- From frame [' +
-                  self.listD[i -
-                             self.paramVecTimeTracks['step']] +
-                  '] to frame [' +
-                  self.listD[i] +
-                  '] -------')
+            print('------- From frame [' + self.listD[i - self.paramVecTimeTracks['step']] + '] to frame [' + self.listD[i] + '] -------')
         if self.processingMode == 'video':
-            print('------- From frame [' +
-                  str(i -
-                      self.paramVecTimeTracks['step']) +
-                  '] to frame [' +
-                  str(i) +
-                  '] -------')
+            print('------- From frame [' + str(i -  self.paramVecTimeTracks['step']) + '] to frame [' + str(i) + '] -------')
         print('Number of Good Feature To Track = ' + str(len(self.X)))
         if len(self.V) == 0:
             print(
                 'No displacements measured (consider changing parameters set if displacements expected between these two frames)')
         else:
-            print('Displacement max = ' + str(np.max(np.absolute(self.V))) +
-                  ' ' + self.unit[0] + '/' + self.unit[1])
+            print('Displacement max = ' + str(np.max(np.absolute(self.V))) +  ' ' + self.unit[0] + '/' + self.unit[1])
 
     def scaleAndLogFlow(self, i):
         if self.scaled:
             self.X = (self.X - np.array(self.origin)) * self.scale
             self.V = self.V * self.scale * self.fps / self.paramVecTime['step']
             self.X[:, 1] = -self.X[:, 1]
             self.V[:, 1] = -self.V[:, 1]
         print('')
         self.incr += 1
         print('-------------- [Step ' + str(self.incr) + ' / ' +
               str(self.paramVecTime['Ntot']) + '] --------------')
         if self.processingMode == 'image sequence':
             print('------- From frame [' +
-                  self.listD[i -
-                             self.paramVecTime['step']] +
-                  '] to frame [' +
-                  self.listD[i] +
-                  '] -------')
+                  self.listD[i - self.paramVecTime['step']] + '] to frame [' + self.listD[i] + '] -------')
         if self.processingMode == 'video':
-            print('------- From frame [' +
-                  str(i -
-                      self.paramVecTime['step']) +
-                  '] to frame [' +
-                  str(i) +
-                  '] -------')
+            print('------- From frame [' + str(i - self.paramVecTime['step']) +  '] to frame [' + str(i) + '] -------')
         print('Number of Good Feature To Track = ' + str(len(self.X)))
         if len(self.V) == 0:
             print(
                 'No displacements measured (consider changing parameters set if displacements expected between these two frames)')
         else:
             print('Displacement max = ' + str(np.max(np.absolute(self.V))) +
                   ' ' + self.unit[0] + '/' + self.unit[1])
@@ -904,37 +860,27 @@
             self.interpolatedVelocities[:, 1], (self.Hgrid, self.Lgrid)))
         self.Field=Render.setField(self.Ux, self.Uy, Type)
         self.Field[np.where(self.Field == 0)]=np.nan
         self.Field=self.Field * self.gridMask
 
         self.fieldResults = 'accumulation'
 
-    def showXV(self,
-            X,
-            V,
-            vis = None,
-            display = 'quiver',
-            displayColor = True,
-            **args):
+    def showXV(self, X, V, vis = None,
+            display = 'quiver', displayColor = True, **args):
         if display == 'quiver' and self.mute == False and self.display == True:
             self.opyfDisp.plotQuiverUnstructured(
                 X, V, vis = vis, displayColor = displayColor, **args)
 
         if display == 'points' and self.mute == False and self.display == True:
             self.opyfDisp.plotPointsUnstructured(
                 Xdata = X, Vdata = V, vis = vis, displayColor = displayColor, **args)
 
-    def scaleData(
-            self,
-            framesPerSecond = None,
+    def scaleData( self, framesPerSecond = None,
             metersPerPx = None,
-            unit = [
-                'm',
-                's'],
-            origin = None):
+            unit = [ 'm', 's'], origin = None):
 
         if self.scaled:
             print('datas already scaled')
         else:
             self.scaled=True
 
             if origin is not None:
@@ -965,17 +911,24 @@
 
             self.grid_y, self.grid_x = (
                 self.grid_y - self.origin[1]) * self.scale, (self.grid_x - self.origin[0]) * self.scale
             self.invertYaxis()
             self.XT = Interpolate.npGrid2TargetPoint2D(
                 self.grid_x, self.grid_y)
 
-            self.interp_params = dict(Radius=self.interp_params['Radius'] * self.scale,  # it is not necessary to perform interpolation on a high radius since we have a high number of values
+            self.interp_params = dict(Radius=self.interp_params['Radius'] * self.scale,  
                                       Sharpness=self.interp_params['Sharpness'],
                                       kernel='Gaussian')
+            self.filters_params['RadiusF'] = self.filters_params['RadiusF']* self.scale
+            self.filters_params['range_Vx'][0] = self.filters_params['range_Vx'][0]* self.scale* self.fps
+            self.filters_params['range_Vx'][1] = self.filters_params['range_Vx'][1]* self.scale* self.fps
+
+            self.filters_params['range_Vy'][0] = self.filters_params['range_Vy'][0]* self.scale* self.fps
+            self.filters_params['range_Vy'][1] = self.filters_params['range_Vy'][1]* self.scale* self.fps
+             
             self.paramPlot = {'vecX': self.vecX,
                               'vecY': self.vecY,
                               'extentFrame': [(self.paramPlot['extentFrame'][0] - self.origin[0]) * self.scale,
                                               (self.paramPlot['extentFrame'][1] - self.origin[0]) * self.scale,
                                               -(self.paramPlot['extentFrame'][2] - self.origin[1]) * self.scale,
                                               -(self.paramPlot['extentFrame'][3] - self.origin[1]) * self.scale,
                                               ],
@@ -1000,16 +953,15 @@
             self.Vaccu = self.Vaccu * np.array([1, -1])
             self.Xdata = [(X * np.array([1, -1])) for X in self.Xdata]
             self.Vdata = [(V * np.array([1, -1])) for V in self.Vdata]
         if hasattr(self, 'UyTot'):
             for i in range(len(self.UyTot)):
                 self.UyTot[i] = -self.UyTot[i]
 
-    def writeGoodFeaturesPositionsAndDisplacements(
-            self,
+    def writeGoodFeaturesPositionsAndDisplacements(self,
             fileFormat='hdf5',
             outFolder='.',
             filename=None,
             fileSequence=False):
         self.filename = filename
 
         if not self.scaled:
@@ -1031,158 +983,89 @@
                     [self.Time, self.Time + self.paramVecTime['step']]).T
                 Files.csv_WriteUnstructured2DTimeserie2(
                     outFolder + '/' + filename + '.' + fileFormat, timeT, XpROI, self.Vdata)
             elif fileSequence:
                 Files.mkdir2(outFolder + '/' + filename)
                 for x, v, t in zip(XpROI, self.Vdata, self.Time):
                     Files.write_csvTrack2D(
-                        outFolder +
-                        '/' +
-                        filename +
-                        '/' +
-                        format(
-                            t,
-                            '04.0f') +
-                        '_to_' +
-                        format(
-                            t +
-                            self.paramVecTime['step'],
-                            '04.0f') +
-                        '.' +
-                        fileFormat,
-                        x,
-                        v)
+                        outFolder + '/' + filename + '/' + format( t,'04.0f') + '_to_' +  format(   t + self.paramVecTime['step'],   '04.0f') + '.' + fileFormat, x, v)
 
         self.writeImageProcessingParamsJSON(outFolder=outFolder)
 
     def writeVelocityField(
             self,
             fileFormat='hdf5',
             outFolder='.',
             filename=None,
             fileSequence=False,
             saveParamsImgProc=True):
         # for export in the image referential only if scaling and origin has
         # not been attributed
         self.filename = filename
         if len(self.UxTot) == 0:
-            sys.exit(
-                '[Warning] the following method should be run to produce an interpolated field that can be saved {extractGoodFeaturesPositionsDisplacementsAndInterpolate} or {extractGoodFeaturesDisplacementsAccumulateAndInterpolate}')
+            sys.exit( '[Warning] the following method should be run to produce an interpolated field that can be saved {extractGoodFeaturesPositionsDisplacementsAndInterpolate} or {extractGoodFeaturesDisplacementsAccumulateAndInterpolate}')
 
         vecXpROI = np.copy(self.vecX)
         vecYpROI = np.copy(self.vecY)
         if not self.scaled:
             vecXpROI = self.vecX + self.ROI[0]
             vecYpROI = self.vecY + self.ROI[1]
 
         self.UxTot = np.array(self.UxTot)
         self.UyTot = np.array(self.UyTot)
 
         if self.fieldResults == 'time-serie':
             if filename is None:
                 self.filename = 'velocity_field_from_frame_' + str(self.vec[0]) + '_to_' + str(self.vec[-1]) + '_with_step_' + str(
                     self.paramVecTime['step']) + '_and_shift_' + str(self.paramVecTime['shift'])
-            self.variables = [['Ux_[' +
-                               self.unit[0] +
-                               '.' +
-                               self.unit[1] +
-                               '-1]', self.UxTot], ['Uy_[' +
-                                                    self.unit[0] +
-                                                    '.' +
-                                                    self.unit[1] +
-                                                    '-1]', self.UyTot]]
+            self.variables = [['Ux_[' + self.unit[0] +'.' +self.unit[1] +
+                               '-1]', self.UxTot], ['Uy_[' +  self.unit[0] +'.' +self.unit[1] + '-1]', self.UyTot]]
             if fileFormat == 'hdf5':
-                Files.hdf5_Write(outFolder +
-                                 '/' +
-                                 self.filename +
-                                 '.' +
-                                 fileFormat, [['T_[' +
-                                               self.unit[0] +
-                                               ']', self.Time], ['X_[' +
-                                                                 self.unit[0] +
-                                                                 ']', vecXpROI], ['Y_[' +
-                                                                                  self.unit[0] +
-                                                                                  ']', vecYpROI]], self.variables)
+                Files.hdf5_Write(outFolder +     '/' +   self.filename +'.' +fileFormat, [['T_[' + self.unit[1] +']', self.Time], ['X_[' +self.unit[0] +']', vecXpROI], ['Y_[' +self.unit[0] +']', vecYpROI]], self.variables)
 
             if fileFormat == 'tecplot' or fileFormat == 'csv' or fileFormat == 'tec':
                 for k in range(len(self.Time)):
                     VT = Interpolate.npGrid2TargetPoint2D(
                         self.UxTot[k], self.UyTot[k])
-                    variablesTecplot = [['Ux_[' +
-                                         self.unit[0] +
-                                         '.' +
-                                         self.unit[1] +
-                                         '^{-1}]', VT[:, 0]], ['Uy_[' +
-                                                               self.unit[0] +
-                                                               '.' +
-                                                               self.unit[1] +
-                                                               '-1]', VT[:, 1]]]
+                    variablesTecplot = [['Ux_[' + self.unit[0] + '.' + self.unit[1] + '^{-1}]', VT[:, 0]], ['Uy_[' + self.unit[0] +  '.' + self.unit[1] +  '-1]', VT[:, 1]]]
                     self.filename = 'velocity_field_from_frame_' + \
                         str(self.vec[2 * k]) + '_to_' + str(self.vec[2 * k + 1])
                     if fileFormat == 'tecplot' or fileFormat == 'tec':
-                        Files.tecplot_WriteRectilinearMesh(str(outFolder +'/' + format(k, '04.0f') +'_' + self.filename + '.' + fileFormat),
-                            vecXpROI,
-                            vecYpROI,
-                            variablesTecplot)
+                        Files.tecplot_WriteRectilinearMesh(str(outFolder +'/' + format(k, '04.0f') +'_' + self.filename + '.' + fileFormat), vecXpROI, vecYpROI, variablesTecplot)
                     if fileFormat == 'csv':
-                        Files.csv_WriteRectilinearMesh(str(outFolder + '/' +  format( k, '04.0f') + '_' + self.filename + '.' + fileFormat),
-                            vecXpROI,
-                            vecYpROI,
-                            variablesTecplot)
+                        Files.csv_WriteRectilinearMesh(str(outFolder + '/' +  format( k, '04.0f') + '_' + self.filename + '.' + fileFormat), vecXpROI, vecYpROI, variablesTecplot)
 
         elif self.fieldResults == 'accumulation':
             VT = Interpolate.npGrid2TargetPoint2D(self.UxTot[0], self.UyTot[0])
             if filename is None:
                 #                filename = 'velocity_field_with_accumulation_of_features_velocities_from_frame_' + str(self.vec[0]) + '_to_' + str(self.vec[-1]) + '_with_step_' + str(
                 # self.paramVecTime['step']) +
                 # '_and_shift_'+str(self.paramVecTime['shift'])
                 self.filename = 'frame_' + str(self.vec[0]) + '_to_' + str(self.vec[-1]) + '_with_step_' + str(
                     self.paramVecTime['step']) + '_and_shift_' + str(self.paramVecTime['shift'])
-            self.variables = [['Ux_[' +
-                               self.unit[0] +
-                               '.' +
-                               self.unit[1] +
-                               '-1]', self.UxTot], ['Uy_[' +
-                                                    self.unit[0] +
-                                                    '.' +
-                                                    self.unit[1] +
-                                                    '-1]', self.UyTot]]
+            self.variables = [['Ux_[' + self.unit[0] + '.' + self.unit[1] +
+                               '-1]', self.UxTot], ['Uy_[' +  self.unit[0] + '.' + self.unit[1] + '-1]', self.UyTot]]
             if fileFormat == 'hdf5':
-                Files.hdf5_Write(outFolder +
-                                 '/' +
-                                 self.filename +
-                                 '.' +
-                                 fileFormat, [['T_[' +
-                                               self.unit[0] +
-                                               ']', self.Time], ['X_[' +
-                                                                 self.unit[0] +
-                                                                 ']', vecXpROI], ['Y_[' +
-                                                                                  self.unit[0] +
-                                                                                  ']', vecYpROI]], self.variables)
+                Files.hdf5_Write(outFolder + '/' + self.filename + '.' +
+                                 fileFormat, [['T_[' +  self.unit[1] + ']', self.Time], ['X_[' + self.unit[0] + ']', vecXpROI], ['Y_[' +  self.unit[0] +']', vecYpROI]], self.variables)
 
             if fileFormat == 'tecplot' or fileFormat == 'csv' or fileFormat == 'tec':
-                variablesTecplot = [['Ux_[' +
-                                     self.unit[0] +
-                                     '.' +
-                                     self.unit[1] +
-                                     '^{-1}]', VT[:, 0]], ['Uy_[' +
-                                                           self.unit[0] +
-                                                           '.' +
-                                                           self.unit[1] +
-                                                           '^{-1}]', VT[:, 1]]]
+                variablesTecplot = [['Ux_[' + self.unit[0] + '.' + self.unit[1] + '^{-1}]', VT[:, 0]], ['Uy_[' +   self.unit[0] +  '.' +  self.unit[1] + '^{-1}]', VT[:, 1]]]
+
                 if fileFormat == 'tecplot' or fileFormat == 'tec':
                     Files.tecplot_WriteRectilinearMesh(
                         outFolder +
                         '/' +
                         self.filename +
                         '.' +
                         fileFormat,
                         vecXpROI,
                         vecYpROI,
                         variablesTecplot)
+
                 if fileFormat == 'csv':
                     Files.csv_WriteRectilinearMesh(
                         outFolder +
                         '/' +
                         self.filename +
                         '.' +
                         fileFormat,
@@ -1201,16 +1084,15 @@
 #                Files.mkdir2(outFolder+'/'+filename)
 #                for x,v,t in zip(self.Xdata,self.Vdata,self.Time):
 #                    Files.write_csvTrack2D(outFolder+'/'+filename+'/'+format(t,'04.0f')+'_to_'+format(t+self.paramVecTime['step'],'04.0f')+'.'+fileFormat,x,v)
 #
 #
 # TODO export this method in Files
 
-    def writeTracks(
-            self,
+    def writeTracks( self,
             filename=None,
             fileFormat='csv',
             outFolder='.',
             saveParamsImgProc=True):
         import csv
         self.filename = filename
         print('')
@@ -1275,20 +1157,17 @@
             'filters_params': self.filters_params,
             'interp_parameter': self.interp_params,
             'vecTime_params': self.paramVecTime}
         fulldict['fieldResults'] = self.fieldResults
         Files.writeImageProcessingParamsJSON(
             fulldict, outFolder=outFolder, filename=None)
 
-    def set_stabilization(
-            self,
+    def set_stabilization( self,
             mask=None,
-            vlim=[
-                0,
-                40],
+            vlim=[  0, 80],
             mute=True,
             close_at_reset=False):
         if mask is None:
             mask = np.ones((self.Hvis, self.Lvis))
         if self.processingMode == 'video':
             self.stab = opyf.videoAnalyzer(
                 self.video_src, mute=mute, display=(
@@ -1309,15 +1188,15 @@
         if s - self.vec[0] > 0:
             self.stab.set_vecTime(
                 Ntot=1,
                 starting_frame=self.vec[0],
                 step=s - self.vec[0])
             self.stab.extractGoodFeaturesAndDisplacements()
             transformation_rigid_matrix, rigid_mask = cv2.estimateAffine2D(
-                self.stab.X + self.stab.V, self.stab.X)
+                self.stab.X + self.stab.V/2, self.stab.X + self.stab.V/2 ) #because the position of the displacement is half the distance btw GFTs
             dst = cv2.warpAffine(
                 self.stab.vis,
                 transformation_rigid_matrix,
                 (self.stab.Lvis,
                  self.stab.Hvis))
             self.vis = dst
         print('-------------Stabilization End -------------')
@@ -1381,54 +1260,43 @@
             model_points, self.rvec1, self.tvec1, camera_matrix, (0, 0, 0, 0))
 
         ax1.scatter(axisPoints[:, 0, 0], axisPoints[:, 0, 1], s=300,
                     linewidths=0.5, marker='P', color=(1, 1, 1, 0.7), zorder=2)
         self.color = []
         props = dict(facecolor=(1, 1, 1), alpha=0.5, pad=2)
         for i in range(len(axisPoints)):
-            self.color.append(
-                [np.random.uniform(), np.random.uniform(), np.random.uniform()])
-            ax1.scatter(axisPoints[i,
-                                   0,
-                                   0],
-                        axisPoints[i,
-                                   0,
-                                   1],
+            self.color.append( [np.random.uniform(), np.random.uniform(), np.random.uniform()])
+            ax1.scatter(axisPoints[i, 0, 0],
+                        axisPoints[i,  0, 1],
                         s=200,
                         linewidths=0.5,
                         marker='+',
                         color=self.color[i],
                         zorder=3)
             ax1.text(axisPoints[i][0,
                                    0],
                      axisPoints[i][0,
                                    1],
                      '        X: ' + format(model_points[i][0],
-                                            '2.2f') + ' m Y: ' + format(model_points[i][1],
-                                                                        '2.2f') + ' m Z: ' + format(model_points[i][2],
-                                                                                                    '2.2f') + ' m   ',
+                                            '2.2f') + ' m Y: ' + format(model_points[i][1],   '2.2f') + ' m Z: ' + format(model_points[i][2], '2.2f') + ' m   ',
                      fontsize=6,
                      bbox=props,
                      zorder=1)
         ax1.set_xlim([0, self.Lvis])
         ax1.set_ylim([self.Hvis, 0])
         # self.opyfDisp.ax.scatter(axisPoints[:,0,0],axisPoints[:,0,1],s=300,linewidths=0.5,marker='P',color=(1,1,1,0.7),zorder=2)
 
         axisPoints, _ = cv2.projectPoints(
             model_points, self.rvec_z, self.tvec_z, camera_matrix, (0, 0, 0, 0))
         ax2.scatter(axisPoints[:, 0, 0], axisPoints[:, 0, 1], s=300,
                     linewidths=0.5, marker='P', color=(1, 1, 1, 0.7), zorder=2)
 
         for i in range(len(axisPoints)):
-            ax2.scatter(axisPoints[i,
-                                   0,
-                                   0],
-                        axisPoints[i,
-                                   0,
-                                   1],
+            ax2.scatter(axisPoints[i,  0,  0],
+                        axisPoints[i,  0,  1],
                         s=200,
                         linewidths=0.5,
                         marker='+',
                         color=self.color[i],
                         zorder=3)
             # ax2.text(axisPoints[i][0,0],
             #   axisPoints[i][0,1],'        X: '+format(model_points[i][0],'2.2f')+' m Y: '+format(model_points[i][1],'2.2f')+' m Z: '+format(model_points[i][2],'2.2f')+' m   ',
@@ -1459,15 +1327,14 @@
                            origin=[axisPoints[0, 0, 0], axisPoints[0, 0, 1]])
         self.birdEyeMod = True
 
         if saveOutPut is not None:
             self.figBET.savefig(saveOutPut)
 
     def transformBirdEye(self):
-
         self.vis = cv2.warpPerspective(
             self.vis, self.homography, (self.Lvis, self.Hvis))
 
 
 # #    plt.subplot(121),plt.imshow(img),plt.title('Input')
 # #    plt.subplot(122),plt.imshow(dst),plt.title('Output')
 # #    plt.show()
```

### Comparing `opyf-1.3/opyf/Files.py` & `opyf-1.4/src/opyf/Files.py`

 * *Files identical despite different names*

### Comparing `opyf-1.3/opyf/Filters.py` & `opyf-1.4/src/opyf/Filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python2
 # -*- coding: utf-8 -*-
 """
 Created on Wed Nov 29 14:58:58 2017
 
 @author: Gauthier ROUSSEAU
 """
+#%%
 
 import vtk
 import numpy as np
 import time
 from vtk.util.numpy_support import vtk_to_numpy
 from tqdm import tqdm
 
@@ -384,7 +385,55 @@
     blob3Dout = np.array(blob3Dout)
     if minArea is not None:
         C = C[np.where(AreaBlob > minArea)]
         blob3Dout = blob3Dout[np.where(AreaBlob > minArea)]
         AreaBlob = AreaBlob[np.where(AreaBlob > minArea)]
 
     return blob3Dout, C, AreaBlob
+
+
+def findClosestPointsTwoLists(X_source,X_target):
+    '''return the closest points indexes in X_source from the X_target points,
+    indexes output has the same length than X_target'''
+
+    listPoints = X_source
+    points = vtk.vtkPoints()
+    points.SetDataTypeToDouble()
+
+    listProbePoints=X_target
+    probePoints = vtk.vtkPoints()
+    probePoints.SetDataTypeToDouble()
+
+
+
+    for [x, y] in listPoints:
+        points.InsertNextPoint(x, y, 0.)
+    for [x, y] in listProbePoints:
+        probePoints.InsertNextPoint(x, y, 0.)
+
+    polydata = vtk.vtkPolyData()
+    polydata.SetPoints(points)
+    points.ComputeBounds()
+
+    staticLocator = vtk.vtkStaticPointLocator()
+    staticLocator.SetDataSet(polydata)
+    staticLocator.SetNumberOfPointsPerBucket(5)
+    staticLocator.AutomaticOn()
+
+    staticLocator.BuildLocator()
+
+    staticClosestN = vtk.vtkIdList()
+    ind = np.zeros(len(X_target), dtype=np.int)
+    D = np.zeros(len(X_target))
+    math = vtk.vtkMath()
+    x = [0, 0, 0]
+    p = [0, 0, 0]
+    staticClosestN = vtk.vtkIdList()
+    for i in range(len(X_target)):
+        staticLocator.FindClosestNPoints(
+            1, probePoints.GetPoint(i), staticClosestN)
+        ind[i] = staticClosestN.GetId(0)  # we then select the closest point
+        points.GetPoint(ind[i], x)
+        probePoints.GetPoint(i, p)
+        D[i] = math.Distance2BetweenPoints(x, p)**0.5
+
+    return ind, D
```

### Comparing `opyf-1.3/opyf/Interpolate.py` & `opyf-1.4/src/opyf/Interpolate.py`

 * *Files identical despite different names*

### Comparing `opyf-1.3/opyf/MeshesAndTime.py` & `opyf-1.4/src/opyf/MeshesAndTime.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,10 +21,12 @@
     return vecTracks, prevTracks
 
 
 
 
 def set_gridToInterpolateOn(pixLeft, pixRight, stepHor, pixUp, pixDown, stepVert):
     grid_y, grid_x = np.mgrid[pixUp:pixDown:stepVert, pixLeft:pixRight:stepHor]
+    grid_y=grid_y+stepVert//2
+    grid_x=grid_x+stepHor//2
     grid_Vx, grid_Vy = np.zeros_like(grid_y), np.zeros_like(grid_x)
     Hgrid, Lgrid = grid_y.shape
     return grid_y, grid_x, grid_Vy, grid_Vx, Hgrid, Lgrid
```

### Comparing `opyf-1.3/opyf/Render.py` & `opyf-1.4/src/opyf/Render.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,19 +130,22 @@
                           'vecX': args.get('vecX', []),
                           'vecY': args.get('vecY', []),
                           'extentFrame': args.get('extentFrame', [0, 1, 0, 1]),
                           'unit': args.get('unit', ['', 'deltaT']),
                           'Hfig': args.get('Hfig', 8),
                           'num': args.get('num', 'opyfPlot'),
                           'grid': args.get('grid', True),
-                          'vlim': args.get('vlim', None)}
+                          'vlim': args.get('vlim', None),
+                          'force_figsize': args.get('force_figsize', None),}
         self.cmap= plt.get_cmap('hot')
         self.reset()
+
         self.fig, self.ax = opyffigureandaxes(
-            extent=self.paramPlot['extentFrame'], Hfig=self.paramPlot['Hfig'], unit=self.paramPlot['unit'][0], num=self.paramPlot['num'])
+            extent=self.paramPlot['extentFrame'], Hfig=self.paramPlot['Hfig'], unit=self.paramPlot['unit'][0], num=self.paramPlot['num'], 
+            force_figsize=self.paramPlot['force_figsize'])
         self.backend=mpl.get_backend()
         self.ax.set_aspect('equal', adjustable='box')
     def reset(self):
         if (len(self.paramPlot['vecX']) > 0 and len(self.paramPlot['vecY']) > 0):
             self.setGridXandGridY(
                 self.paramPlot['vecX'], self.paramPlot['vecY'])
 
@@ -163,15 +166,15 @@
 
     def setExtent(self, extent):
         self.ax.set_xlim(extent[0], extent[1])
         self.ax.set_ylim(extent[2], extent[3])
         self.paramPlot['extentFrame'] = extent
 
     def opyfColorBar(self,label='Magnitude [px/Dt]', **args):
-        self.cbaxes = self.fig.add_axes([0.15, 0.1, 0.70, 0.03])
+        self.cbaxes = self.fig.add_axes([0.15, 0.15, 0.70, 0.03])
         self.cb = self.fig.colorbar(self.im, cax=self.cbaxes, orientation='horizontal', **args)
         self.cb.set_label(label)
 
 
     def opyfField(self,grid_val, dConfig=None, extent=None, extentr=None, **args):
        
         if 'vlim' in args:
@@ -358,41 +361,50 @@
         norm.vmin = vlim[0]
         norm.vmax = vlim[1]
         self.im = mpl.cm.ScalarMappable(cmap=cmap, norm=norm)
         self.im.set_array([])
         if self.ax.get_ylim()[0] > self.ax.get_ylim()[1]:
             Velocities[:, 1] = -Velocities[:, 1]
         if normalize == False:
-            qv = self.ax.quiver(TargetPoints[:, 0], TargetPoints[:, 1], Velocities[:,
+            self.qv = self.ax.quiver(TargetPoints[:, 0], TargetPoints[:, 1], Velocities[:,
                                                                             0], Velocities[:, 1], color=cmap(norm(Norme)), **args)
         else:
-            qv = self.ax.quiver(TargetPoints[:, 0], TargetPoints[:, 1], Velocities[:, 0] /
+            self.qv = self.ax.quiver(TargetPoints[:, 0], TargetPoints[:, 1], Velocities[:, 0] /
                         Norme[:], Velocities[:, 1]/Norme[:], color=cmap(norm(Norme)), **args)
 
 
 
 
     def plot(self, Field=None,
              gridVx=None, gridVy=None,
              Xdata=None, Vdata=None,
              vis=None, Ptype='norm', Hfig=8,
              namefig='Opyf', scale=None, cmap=None,
              alpha=0.6, width=0.002, nvec=3000, res=32,
              c='k', s=10, ROIvis=None, **args):
 
         if len(self.ax.collections) > 0:
-            del self.ax.collections[:]
+            for c in self.ax.collections:
+                c.remove()
         if len(self.ax.lines) > 0:
-            del self.ax.lines[:]
+            for c in self.ax.lines:
+                c.remove()
         if len(self.ax.images) > 0:
-            del self.ax.images[:]
+            for c in self.ax.images:
+                c.remove()
         if len(self.ax.texts) > 0:
-            del self.ax.texts[:]
+            for c in self.ax.texts:
+                c.remove()
+        if len(self.ax.patches) > 0:
+            for c in self.ax.patches:
+                c.remove()
         if len(self.fig.axes) > 1:
             self.fig.axes[1].remove()
+
+
         if self.backend[-14:]== 'backend_inline' or self.backend[-14:]== 'nbAgg' :  
             self.fig, self.ax = opyffigureandaxes(
             extent=self.paramPlot['extentFrame'], Hfig=self.paramPlot['Hfig'], unit=self.paramPlot['unit'][0], num=self.paramPlot['num'])
 
 
 #            self.fig,self.ax= opyffigureandaxes(extent=self.paramPlot['extentFrame'],Hfig=self.paramPlot['Hfig'],unit=self.paramPlot['unit'][0],num='opfPlot')
 
@@ -453,36 +465,37 @@
             self.cb.set_alpha(0.8)
             self.cb.draw_all()
     #
         if self.paramDisp['DisplayPoints'] == True and Xdata is not None and Vdata is not None:
             self.opyfPointCloudScatter(Xdata, Vdata, s=s, color=c, **infoPlotPointCloud)
 
         if self.paramDisp['QuiverOnPoints'] == True and Xdata is not None and Vdata is not None:
-            self.fig, self.ax, qv = opyfQuiverPointCloud(
+            self.fig, self.ax, self.qv = opyfQuiverPointCloud(
                 Xdata, Vdata, ax=self.ax, nvec=nvec, color=c, normalize=normalize, **infoPlotQuiver)
 
         if self.paramDisp['QuiverOnPointsColored'] == True and Xdata is not None and Vdata is not None:
             self.opyfQuiverPointCloudColored(
                 Xdata, Vdata, nvec=nvec, normalize=normalize, **infoPlotQuiver)
             self.opyfColorBar(
                  label=Ptype+' velocity (in '+self.paramPlot['unit'][0]+'/'+self.paramPlot['unit'][1] + ')')
             self.cb.set_alpha(0.8)
             self.cb.draw_all()
         
         # self.fig.show()
+
         self.fig.canvas.draw()
         self.fig.canvas.start_event_loop(0.01)
         self.fig.canvas.flush_events()
         if self.backend[-14:]== 'backend_inline' or self.backend[-14:]== 'nbAgg' :  
             plt.pause(0.05)
+        
 
     def FieldInitializer(self, vecX, vecY, Field):
         if (len(self.paramPlot['vecX']) == 0 and vecX is not None and vecY is None) or (len(self.paramPlot['vecX']) == 0 and vecX is not None and vecY is None):
-            print(
-                'If you initialize with new coordinates you must specifiy vecX and vecY')
+            print('If you initialize with new coordinates you must specifiy vecX and vecY')
         if len(self.paramPlot['vecX']) == 0 and vecX is not None and vecY is not None:
             self.paramPlot['vecX'] = vecX
             self.paramPlot['vecY'] = vecY
             plt.close('all')
             self.fig, self.ax = opyffigureandaxes(
                 extent=self.paramPlot['extentFrame'], Hfig=self.paramPlot['Hfig'], unit=self.paramPlot['unit'][0], num='opyfPlot')
 
@@ -927,21 +940,21 @@
     fig, ax = getax(fig=fig, ax=ax)
     ax.plot(X[:, 0], X[:, 1], '.', **args)
 
     return fig, ax
 
 
 def opyfColorBar(fig, im, label='Magnitude [px/Dt]', **args):
-    cbaxes = fig.add_axes([0.15, 0.1, 0.70, 0.03])
+    cbaxes = fig.add_axes([0.15, 0.3, 0.70, 0.03])
     cb = fig.colorbar(im, cax=cbaxes, orientation='horizontal', **args)
     cb.set_label(label)
     return fig, cb
 
 
-def opyffigureandaxes(extent=[0, 1, 0, 1], unit='px', Hfig=8, sizemax=15, **args):
+def opyffigureandaxes(extent=[0, 1, 0, 1], unit='px', Hfig=8,  sizemax=15, force_figsize=None, **args):
     Hframe = np.absolute(extent[3]-extent[2])
     Lframe = np.absolute(extent[1]-extent[0])
     Lfig = Lframe*Hfig/Hframe
     # Location of the plot
 #    coefy=0.0004
 
     num = args.get('num', 'opyfPlot')
@@ -949,17 +962,18 @@
         plt.close(num)
     A = np.array([Lfig, Hfig])
     if np.max(A) > sizemax:
         coeff = sizemax/A[np.argmax(A)]
         A = coeff*A
     exty = 0.65
     extx = Lframe*exty*A[1]/A[0]/Hframe
-    axiswindow = [(1-extx)/2+0.02, 0.25, extx, exty]
-
-    fig = plt.figure(figsize=(A[0], A[1]), dpi=142,**args)
+    axiswindow = [(1-extx)/2+0.02, 0.3, extx, exty]
+    if force_figsize is not None:
+        A=force_figsize
+    fig = plt.figure(figsize=(A[0], A[1]), dpi=142, **args)
     ax = plt.Axes(fig, axiswindow)
     fig.add_axes(ax)
     ax.set_ylabel('Y ['+unit+']')
     ax.set_xlabel('X ['+unit+']')
     ax.axis('equal')
     ax.set_xlim(extent[0], extent[1])
     ax.set_ylim(extent[2], extent[3])
```

### Comparing `opyf-1.3/opyf/Track.py` & `opyf-1.4/src/opyf/Track.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 continue
             norm = (vx**2+vy**2)**0.5
             if norm < vmin or norm > vmax:
                 continue
             if maskFrame is not None:
                 if maskFrame[int(y), int(x)] == 0:
                     continue
-            tr.append((x+vx/2, y+vy/2))
+            tr.append((x, y))
             vtr.append((vx, vy))
             if len(tr) > tracks_params['track_len']:
                 del tr[0]
                 del vtr[0]
             new_tracks.append(tr)
             new_vtracks.append(vtr)
         tracks = new_tracks
```

### Comparing `opyf-1.3/opyf/custom_cmap.py` & `opyf-1.4/src/opyf/custom_cmap.py`

 * *Files identical despite different names*

```diff
@@ -26,15 +26,15 @@
     a cmap with equally spaced colors.
     Arrange your tuples so that the first color is the lowest value for the
     colorbar and the last is the highest.
     position contains values from 0 to 1 to dictate the location of each color.
     '''
     import matplotlib as mpl
 
-    bit_rgb = np.linspace(0, 1, res)
+    bit_rgb = np.linspace(0, 1, 256)
     if position == None:
         position = np.linspace(0, 1, len(colors))
     else:
         if len(position) != len(colors):
             sys.exit("position length must be the same as colors")
         elif position[0] != 0 or position[-1] != 1:
             sys.exit("position must start with 0 and end with 1")
```

