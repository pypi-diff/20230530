# Comparing `tmp/plot-antenna-1.4.tar.gz` & `tmp/plot-antenna-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plot-antenna-1.4.tar", last modified: Tue May 30 14:38:50 2023, max compression
+gzip compressed data, was "plot-antenna-1.5.tar", last modified: Tue May 30 20:03:16 2023, max compression
```

## Comparing `plot-antenna-1.4.tar` & `plot-antenna-1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-30 14:38:50.137074 plot-antenna-1.4/
--rw-r--r--   0 ralf      (1000) priv      (1011)    10454 2023-05-30 14:38:50.133074 plot-antenna-1.4/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)     8374 2023-05-30 14:36:39.000000 plot-antenna-1.4/README.rst
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-30 14:38:50.101074 plot-antenna-1.4/plot_antenna/
--rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-05-30 14:37:55.000000 plot-antenna-1.4/plot_antenna/Version.py
--rw-r--r--   0 ralf      (1000) priv      (1011)        0 2022-09-11 10:43:22.000000 plot-antenna-1.4/plot_antenna/__init__.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)    49702 2023-05-30 14:31:49.000000 plot-antenna-1.4/plot_antenna/plot_antenna.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-30 14:38:50.125074 plot-antenna-1.4/plot_antenna.egg-info/
--rw-r--r--   0 ralf      (1000) priv      (1011)    10454 2023-05-30 14:38:50.000000 plot-antenna-1.4/plot_antenna.egg-info/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)      333 2023-05-30 14:38:50.000000 plot-antenna-1.4/plot_antenna.egg-info/SOURCES.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-05-30 14:38:50.000000 plot-antenna-1.4/plot_antenna.egg-info/dependency_links.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       65 2023-05-30 14:38:50.000000 plot-antenna-1.4/plot_antenna.egg-info/entry_points.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       17 2023-05-30 14:38:50.000000 plot-antenna-1.4/plot_antenna.egg-info/requires.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       13 2023-05-30 14:38:50.000000 plot-antenna-1.4/plot_antenna.egg-info/top_level.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-05-30 14:38:50.137074 plot-antenna-1.4/setup.cfg
--rw-r--r--   0 ralf      (1000) priv      (1011)     2716 2022-09-13 14:27:54.000000 plot-antenna-1.4/setup.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-30 14:38:50.129074 plot-antenna-1.4/test/
--rw-r--r--   0 ralf      (1000) priv      (1011)     7225 2022-09-13 13:39:50.000000 plot-antenna-1.4/test/test_plot.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-30 20:03:16.499867 plot-antenna-1.5/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    10664 2023-05-30 20:03:16.499867 plot-antenna-1.5/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)     8544 2023-05-30 20:00:47.000000 plot-antenna-1.5/README.rst
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-30 20:03:16.467867 plot-antenna-1.5/plot_antenna/
+-rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-05-30 20:02:20.000000 plot-antenna-1.5/plot_antenna/Version.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)        0 2022-09-11 10:43:22.000000 plot-antenna-1.5/plot_antenna/__init__.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)    50599 2023-05-30 19:59:11.000000 plot-antenna-1.5/plot_antenna/plot_antenna.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-30 20:03:16.491867 plot-antenna-1.5/plot_antenna.egg-info/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    10664 2023-05-30 20:03:16.000000 plot-antenna-1.5/plot_antenna.egg-info/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)      333 2023-05-30 20:03:16.000000 plot-antenna-1.5/plot_antenna.egg-info/SOURCES.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-05-30 20:03:16.000000 plot-antenna-1.5/plot_antenna.egg-info/dependency_links.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       65 2023-05-30 20:03:16.000000 plot-antenna-1.5/plot_antenna.egg-info/entry_points.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       17 2023-05-30 20:03:16.000000 plot-antenna-1.5/plot_antenna.egg-info/requires.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       13 2023-05-30 20:03:16.000000 plot-antenna-1.5/plot_antenna.egg-info/top_level.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-05-30 20:03:16.499867 plot-antenna-1.5/setup.cfg
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2716 2022-09-13 14:27:54.000000 plot-antenna-1.5/setup.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-30 20:03:16.495867 plot-antenna-1.5/test/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     7225 2022-09-13 13:39:50.000000 plot-antenna-1.5/test/test_plot.py
```

### Comparing `plot-antenna-1.4/PKG-INFO` & `plot-antenna-1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plot-antenna
-Version: 1.4
+Version: 1.5
 Summary: Antenna plotting program for plotting antenna simulation results
 Home-page: https://github.com/schlatterbeck/plot-antenna
 Author: Ralf Schlatterbeck
 Author-email: rsc@runtux.com
 License: MIT License
 Description: Antenna Plotting Program
         ========================
@@ -153,14 +153,19 @@
         .. _matplotlib: https://matplotlib.org/
         .. _plotly: https://github.com/plotly/plotly.py
         .. _pandas: https://pandas.pydata.org/
         
         Release Notes
         -------------
         
+        v1.5: Allow target SWR frequency in VSWR plot
+        
+        - Add command-line option --target-swr-frequency
+        - Draw user-specifed target frequency in red, best (minimum) swr in grey
+        
         v1.4: Reset button and VSWR-Plot improvements
         
         - Add grid and minimum-SWR vertical line to VSWR plot
         - Remove display of frequency in mouse-over (in polar plots and 3D plot)
         - Make polar reset button reset more parameters
         
         v1.3: Add a reset button to plotly polar plots
```

### Comparing `plot-antenna-1.4/README.rst` & `plot-antenna-1.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,19 @@
 .. _matplotlib: https://matplotlib.org/
 .. _plotly: https://github.com/plotly/plotly.py
 .. _pandas: https://pandas.pydata.org/
 
 Release Notes
 -------------
 
+v1.5: Allow target SWR frequency in VSWR plot
+
+- Add command-line option --target-swr-frequency
+- Draw user-specifed target frequency in red, best (minimum) swr in grey
+
 v1.4: Reset button and VSWR-Plot improvements
 
 - Add grid and minimum-SWR vertical line to VSWR plot
 - Remove display of frequency in mouse-over (in polar plots and 3D plot)
 - Make polar reset button reset more parameters
 
 v1.3: Add a reset button to plotly polar plots
```

### Comparing `plot-antenna-1.4/plot_antenna/plot_antenna.py` & `plot-antenna-1.5/plot_antenna/plot_antenna.py`

 * *Files 1% similar despite different names*

```diff
@@ -1017,35 +1017,49 @@
             gd  = self.gdata [f]
             z   = gd.impedance
             rho = np.abs ((z - z0) / (z + z0))
             X.append (f)
             Y.append ((1 + rho) / (1 - rho))
         min_idx = np.argmin (Y)
         self.min_x = X [min_idx]
+        if self.args.target_swr_frequency:
+            if not X [0] <= self.args.target_swr_frequency <= X [-1]:
+                print \
+                    ( "Warning: SWR target frequency %.2f not in range, ignored"
+                    % self.args.target_swr_frequency
+                    , file = sys.stderr
+                    )
+                self.args.target_swr_frequency = None
         return X, Y
     # end def prepare_vswr
 
     def plot_vswr_matplotlib (self, name):
         ax = self.axes [name]
         ax.set_xlabel ('Frequency')
         ax.set_ylabel ('VSWR')
         X, Y = self.prepare_vswr ()
         ax.plot (X, Y)
         ax.grid (color = '0.95')
-        ax.axvline (x = self.min_x, color = 'r', linestyle = 'dashed')
+        tg = self.args.target_swr_frequency
+        if tg is not None:
+            ax.axvline (x = tg, color = 'r', linestyle = 'dashed')
+        ax.axvline (x = self.min_x, color = 'grey', linestyle = 'dashed')
     # end def plot_vswr_matplotlib
 
     def plot_vswr_plotly (self, name):
         X, Y = self.prepare_vswr ()
         df = pd.DataFrame ()
         df ['Frequency'] = X
         df ['VSWR'] = Y
         fig = px.line (df, x="Frequency", y="VSWR")
         fig.update (self.plotly_line_default)
-        fig.add_vline (x = self.min_x, line_dash = "dash", line_color = "red")
+        tg = self.args.target_swr_frequency
+        if tg is not None:
+            fig.add_vline (x = tg, line_dash = "dash", line_color = "red")
+        fig.add_vline (x = self.min_x, line_dash = "dash", line_color = "grey")
         self.show_plotly (fig, name)
     # end def plot_vswr_plotly
 
     def scene_ranges (self, matrix = None):
         """ Create cubic bounding box to force equal aspect ratio
             If matrix is not given, we concatenate *all* gains.
         """
@@ -1276,14 +1290,20 @@
         )
     cmd.add_argument \
         ( '--plot-vswr', '--swr', '--vswr', '--plot-swr'
         , help    = 'Plot voltage standing wave ratio (VSWR)'
         , action  = 'store_true'
         )
     cmd.add_argument \
+        ( "--target-swr-frequency", "--target-vswr-frequency"
+        , help    = "In SWR plot, draw a red vertical line at this "
+                    "frequency"
+        , type    = float
+        )
+    cmd.add_argument \
         ( '--title-font-size'
         , help    = 'Title/legend font size in pt '
                     '(currently only used in plotly)'
         , type    = int
         )
     cmd.add_argument \
         ( '--wireframe'
```

### Comparing `plot-antenna-1.4/plot_antenna.egg-info/PKG-INFO` & `plot-antenna-1.5/plot_antenna.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plot-antenna
-Version: 1.4
+Version: 1.5
 Summary: Antenna plotting program for plotting antenna simulation results
 Home-page: https://github.com/schlatterbeck/plot-antenna
 Author: Ralf Schlatterbeck
 Author-email: rsc@runtux.com
 License: MIT License
 Description: Antenna Plotting Program
         ========================
@@ -153,14 +153,19 @@
         .. _matplotlib: https://matplotlib.org/
         .. _plotly: https://github.com/plotly/plotly.py
         .. _pandas: https://pandas.pydata.org/
         
         Release Notes
         -------------
         
+        v1.5: Allow target SWR frequency in VSWR plot
+        
+        - Add command-line option --target-swr-frequency
+        - Draw user-specifed target frequency in red, best (minimum) swr in grey
+        
         v1.4: Reset button and VSWR-Plot improvements
         
         - Add grid and minimum-SWR vertical line to VSWR plot
         - Remove display of frequency in mouse-over (in polar plots and 3D plot)
         - Make polar reset button reset more parameters
         
         v1.3: Add a reset button to plotly polar plots
```

### Comparing `plot-antenna-1.4/setup.py` & `plot-antenna-1.5/setup.py`

 * *Files identical despite different names*

### Comparing `plot-antenna-1.4/test/test_plot.py` & `plot-antenna-1.5/test/test_plot.py`

 * *Files identical despite different names*

