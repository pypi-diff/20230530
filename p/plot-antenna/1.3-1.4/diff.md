# Comparing `tmp/plot-antenna-1.3.tar.gz` & `tmp/plot-antenna-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plot-antenna-1.3.tar", last modified: Sat May 13 14:56:25 2023, max compression
+gzip compressed data, was "plot-antenna-1.4.tar", last modified: Tue May 30 14:38:50 2023, max compression
```

## Comparing `plot-antenna-1.3.tar` & `plot-antenna-1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-13 14:56:25.095480 plot-antenna-1.3/
--rw-r--r--   0 ralf      (1000) priv      (1011)    10183 2023-05-13 14:56:25.091480 plot-antenna-1.3/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)     8151 2023-05-13 14:54:56.000000 plot-antenna-1.3/README.rst
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-13 14:56:25.063480 plot-antenna-1.3/plot_antenna/
--rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-05-13 14:55:53.000000 plot-antenna-1.3/plot_antenna/Version.py
--rw-r--r--   0 ralf      (1000) priv      (1011)        0 2022-09-11 10:43:22.000000 plot-antenna-1.3/plot_antenna/__init__.py
--rwxr-xr-x   0 ralf      (1000) priv      (1011)    48877 2023-05-09 18:37:00.000000 plot-antenna-1.3/plot_antenna/plot_antenna.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-13 14:56:25.087480 plot-antenna-1.3/plot_antenna.egg-info/
--rw-r--r--   0 ralf      (1000) priv      (1011)    10183 2023-05-13 14:56:24.000000 plot-antenna-1.3/plot_antenna.egg-info/PKG-INFO
--rw-r--r--   0 ralf      (1000) priv      (1011)      333 2023-05-13 14:56:25.000000 plot-antenna-1.3/plot_antenna.egg-info/SOURCES.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-05-13 14:56:24.000000 plot-antenna-1.3/plot_antenna.egg-info/dependency_links.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       65 2023-05-13 14:56:24.000000 plot-antenna-1.3/plot_antenna.egg-info/entry_points.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       17 2023-05-13 14:56:24.000000 plot-antenna-1.3/plot_antenna.egg-info/requires.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       13 2023-05-13 14:56:24.000000 plot-antenna-1.3/plot_antenna.egg-info/top_level.txt
--rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-05-13 14:56:25.095480 plot-antenna-1.3/setup.cfg
--rw-r--r--   0 ralf      (1000) priv      (1011)     2716 2022-09-13 14:27:54.000000 plot-antenna-1.3/setup.py
-drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-13 14:56:25.087480 plot-antenna-1.3/test/
--rw-r--r--   0 ralf      (1000) priv      (1011)     7225 2022-09-13 13:39:50.000000 plot-antenna-1.3/test/test_plot.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-30 14:38:50.137074 plot-antenna-1.4/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    10454 2023-05-30 14:38:50.133074 plot-antenna-1.4/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)     8374 2023-05-30 14:36:39.000000 plot-antenna-1.4/README.rst
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-30 14:38:50.101074 plot-antenna-1.4/plot_antenna/
+-rw-r--r--   0 ralf      (1000) priv      (1011)       14 2023-05-30 14:37:55.000000 plot-antenna-1.4/plot_antenna/Version.py
+-rw-r--r--   0 ralf      (1000) priv      (1011)        0 2022-09-11 10:43:22.000000 plot-antenna-1.4/plot_antenna/__init__.py
+-rwxr-xr-x   0 ralf      (1000) priv      (1011)    49702 2023-05-30 14:31:49.000000 plot-antenna-1.4/plot_antenna/plot_antenna.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-30 14:38:50.125074 plot-antenna-1.4/plot_antenna.egg-info/
+-rw-r--r--   0 ralf      (1000) priv      (1011)    10454 2023-05-30 14:38:50.000000 plot-antenna-1.4/plot_antenna.egg-info/PKG-INFO
+-rw-r--r--   0 ralf      (1000) priv      (1011)      333 2023-05-30 14:38:50.000000 plot-antenna-1.4/plot_antenna.egg-info/SOURCES.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)        1 2023-05-30 14:38:50.000000 plot-antenna-1.4/plot_antenna.egg-info/dependency_links.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       65 2023-05-30 14:38:50.000000 plot-antenna-1.4/plot_antenna.egg-info/entry_points.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       17 2023-05-30 14:38:50.000000 plot-antenna-1.4/plot_antenna.egg-info/requires.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       13 2023-05-30 14:38:50.000000 plot-antenna-1.4/plot_antenna.egg-info/top_level.txt
+-rw-r--r--   0 ralf      (1000) priv      (1011)       38 2023-05-30 14:38:50.137074 plot-antenna-1.4/setup.cfg
+-rw-r--r--   0 ralf      (1000) priv      (1011)     2716 2022-09-13 14:27:54.000000 plot-antenna-1.4/setup.py
+drwxr-xr-x   0 ralf      (1000) priv      (1011)        0 2023-05-30 14:38:50.129074 plot-antenna-1.4/test/
+-rw-r--r--   0 ralf      (1000) priv      (1011)     7225 2022-09-13 13:39:50.000000 plot-antenna-1.4/test/test_plot.py
```

### Comparing `plot-antenna-1.3/PKG-INFO` & `plot-antenna-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plot-antenna
-Version: 1.3
+Version: 1.4
 Summary: Antenna plotting program for plotting antenna simulation results
 Home-page: https://github.com/schlatterbeck/plot-antenna
 Author: Ralf Schlatterbeck
 Author-email: rsc@runtux.com
 License: MIT License
 Description: Antenna Plotting Program
         ========================
@@ -153,14 +153,20 @@
         .. _matplotlib: https://matplotlib.org/
         .. _plotly: https://github.com/plotly/plotly.py
         .. _pandas: https://pandas.pydata.org/
         
         Release Notes
         -------------
         
+        v1.4: Reset button and VSWR-Plot improvements
+        
+        - Add grid and minimum-SWR vertical line to VSWR plot
+        - Remove display of frequency in mouse-over (in polar plots and 3D plot)
+        - Make polar reset button reset more parameters
+        
         v1.3: Add a reset button to plotly polar plots
         
         - The polar plots, when zoomed in, could only be reset to the unzoomed
           view with a double-click. All other plots do have a reset button, add
           one for the polar plots, too.
         
         v1.2: Allow specification of title (legend) font size in plotly version
```

### Comparing `plot-antenna-1.3/README.rst` & `plot-antenna-1.4/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -145,14 +145,20 @@
 .. _matplotlib: https://matplotlib.org/
 .. _plotly: https://github.com/plotly/plotly.py
 .. _pandas: https://pandas.pydata.org/
 
 Release Notes
 -------------
 
+v1.4: Reset button and VSWR-Plot improvements
+
+- Add grid and minimum-SWR vertical line to VSWR plot
+- Remove display of frequency in mouse-over (in polar plots and 3D plot)
+- Make polar reset button reset more parameters
+
 v1.3: Add a reset button to plotly polar plots
 
 - The polar plots, when zoomed in, could only be reset to the unzoomed
   view with a double-click. All other plots do have a reset button, add
   one for the polar plots, too.
 
 v1.2: Allow specification of title (legend) font size in plotly version
```

### Comparing `plot-antenna-1.3/plot_antenna/plot_antenna.py` & `plot-antenna-1.4/plot_antenna/plot_antenna.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,14 +271,16 @@
 # end def nearest_angle_idx
 
 class Gain_Plot:
     fig_x = 512
     fig_y = 384
     plot_names   = ('azimuth', 'elevation', 'plot_vswr', 'plot3d', 'plot_geo')
     update_names = set (('azimuth', 'elevation', 'plot3d'))
+    font_sans    = \
+        "Helvetica, Nimbus Sans, Liberation Sans, Open Sans, arial, sans-serif"
 
 
     def __init__ (self, args):
         self.args        = args
         self.dpi         = args.dpi
         self.filename    = args.filename
         self.outfile     = args.output_file
@@ -369,15 +371,15 @@
                         , linecolor = "#B0B0B0"
                         , gridcolor = "#B0B0B0"
                         )
                     , bgcolor = '#FFFFFF'
                     )
                 , title = dict
                     ( font = dict
-                        ( family = "Helvetica"
+                        ( family = self.font_sans
                         , color  = "#010101"
                         )
                     )
                 )
             )
         return d
     # end def plotly_polar_default
@@ -386,19 +388,19 @@
     def plotly_line_default (self):
         d = dict \
             ( layout = dict
                 ( showlegend = True
                 , colorway   = self.colormap
                 , xaxis = dict
                     ( linecolor = "#B0B0B0"
-                    , gridcolor = "white"
+                    , gridcolor = "#F2F2F2"
                     )
                 , yaxis = dict
                     ( linecolor = "#B0B0B0"
-                    , gridcolor = "white"
+                    , gridcolor = "#F2F2F2"
                     )
                 , paper_bgcolor = 'white'
                 , plot_bgcolor  = 'white'
                 )
             )
         return d
     # end def plotly_line_default
@@ -784,35 +786,42 @@
             Plotly.relayout (myPlot,
                 {'modebar':
                     { 'add' :
                         [   { 'name'  : 'Reset'
                             , 'icon'  : Plotly.Icons.home
                             , 'click' : function (gd)
                               { Plotly.relayout
-                                (gd, {'polar.radialaxis.range': [0,1]});
+                                ( gd
+                                , { 'polar.radialaxis.range': [0,1]
+                                  , 'polar.radialaxis.angle': %(lbl_deg)s
+                                  , 'polar.radialaxis.tickangle' : %(tickangle)s
+                                  , 'polar.angularaxis.rotation' : 0
+                                  }
+                                );
                               }
                             }
                         ]
                     }
                 });
             """
 
     def polarplot_plotly (self, name):
         fig = self.plotly_fig
         nm  = self.angle_name
+        tpl = 'Gain: %%{text}<br>%s: %%{theta}<extra></extra>' % nm
         df = dict \
             ( r       = self.polargains
             , theta   = (self.angles / np.pi * 180) % 360
             , name    = "f=%.3f MHz" % self.frequency
             , mode    = 'lines'
             , visible = True if self.plotly_firstfig else 'legendonly'
             , text    = ['%.2f dBi (%.2f dB)' % (u, u - self.maxg)
                          for u in self.unscaled
                         ]
-            , hovertemplate = 'Gain: %%{text}<br>%s: %%{theta}' % nm
+            , hovertemplate = tpl
             )
         fig.add_trace (go.Scatterpolar (**df))
         if self.plotly_lastfig:
             desc = '<br>'.join (self.desc [0:2] + self.desc [3:])
             # don't use fig.update_layout (title = desc) which will
             # delete title attributes
             fig.layout.title.text = desc
@@ -820,14 +829,15 @@
                 fig.layout.title.font.size = self.args.title_font_size
             lbl_deg = self.lbl_deg or 0
             tickangle = 90
             if lbl_deg > 180:
                 tickangle = -90
             fig.layout.polar.radialaxis.tickangle = tickangle
             fig.layout.polar.radialaxis.angle = lbl_deg
+            fig.layout.polar.radialaxis.range = [0,1]
 # Trying to display 'X' and 'Y' on Azimuth plot
 # Doesn't work: This doesn't correctly scale and it seems giving
 # annotations in polar coordinates is still not possible
 #            if self.labels:
 #                fig.add_annotation \
 #                    ( xref      = 'x domain'
 #                    , yref      = 'y domain'
@@ -844,15 +854,16 @@
 #                    , x         = 0.5
 #                    , y         = 1.1
 #                    , showarrow = False
 #                    , align     = 'center'
 #                    , text      = self.labels [1]
 #                    , font      = dict (size = 18)
 #                    )
-            self.show_plotly (fig, name, script = self.plotly_polar_script)
+            script = self.plotly_polar_script % locals ()
+            self.show_plotly (fig, name, script = script)
     # end def polarplot_plotly
 
     def polarplot_matplotlib (self, name):
         if name not in self.gui_objects:
             self.gui_objects [name] = {}
         ax = self.axes [name]
         ax.set_rmax (1)
@@ -942,15 +953,15 @@
         # different frequencies
         tickvals = self.scaler.tick_values
         tickvals [0] = gains.max ()
         lgroup  = 'l%d' % self.plotly_count
         visible = True if self.plotly_firstfig else 'legendonly'
         tpl = ('Gain: %{customdata[0]:.2f} dBi (%{customdata[1]:.2f} dB)<br>'
                'Azimuth: %{customdata[2]:.2f}° (X: 0°)<br>'
-               'Elevation: %{customdata[3]:.2f}°'
+               'Elevation: %{customdata[3]:.2f}°<extra></extra>'
               )
 
         fig.add_trace \
             ( go.Surface
                 ( x = X, y = Y, z = Z
                 , surfacecolor = gains
                 , colorscale   = 'rainbow'
@@ -1004,32 +1015,37 @@
         Y  = []
         for f in self.gdata:
             gd  = self.gdata [f]
             z   = gd.impedance
             rho = np.abs ((z - z0) / (z + z0))
             X.append (f)
             Y.append ((1 + rho) / (1 - rho))
+        min_idx = np.argmin (Y)
+        self.min_x = X [min_idx]
         return X, Y
     # end def prepare_vswr
 
     def plot_vswr_matplotlib (self, name):
         ax = self.axes [name]
         ax.set_xlabel ('Frequency')
         ax.set_ylabel ('VSWR')
         X, Y = self.prepare_vswr ()
         ax.plot (X, Y)
+        ax.grid (color = '0.95')
+        ax.axvline (x = self.min_x, color = 'r', linestyle = 'dashed')
     # end def plot_vswr_matplotlib
 
     def plot_vswr_plotly (self, name):
         X, Y = self.prepare_vswr ()
         df = pd.DataFrame ()
         df ['Frequency'] = X
         df ['VSWR'] = Y
         fig = px.line (df, x="Frequency", y="VSWR")
         fig.update (self.plotly_line_default)
+        fig.add_vline (x = self.min_x, line_dash = "dash", line_color = "red")
         self.show_plotly (fig, name)
     # end def plot_vswr_plotly
 
     def scene_ranges (self, matrix = None):
         """ Create cubic bounding box to force equal aspect ratio
             If matrix is not given, we concatenate *all* gains.
         """
```

### Comparing `plot-antenna-1.3/plot_antenna.egg-info/PKG-INFO` & `plot-antenna-1.4/plot_antenna.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plot-antenna
-Version: 1.3
+Version: 1.4
 Summary: Antenna plotting program for plotting antenna simulation results
 Home-page: https://github.com/schlatterbeck/plot-antenna
 Author: Ralf Schlatterbeck
 Author-email: rsc@runtux.com
 License: MIT License
 Description: Antenna Plotting Program
         ========================
@@ -153,14 +153,20 @@
         .. _matplotlib: https://matplotlib.org/
         .. _plotly: https://github.com/plotly/plotly.py
         .. _pandas: https://pandas.pydata.org/
         
         Release Notes
         -------------
         
+        v1.4: Reset button and VSWR-Plot improvements
+        
+        - Add grid and minimum-SWR vertical line to VSWR plot
+        - Remove display of frequency in mouse-over (in polar plots and 3D plot)
+        - Make polar reset button reset more parameters
+        
         v1.3: Add a reset button to plotly polar plots
         
         - The polar plots, when zoomed in, could only be reset to the unzoomed
           view with a double-click. All other plots do have a reset button, add
           one for the polar plots, too.
         
         v1.2: Allow specification of title (legend) font size in plotly version
```

### Comparing `plot-antenna-1.3/setup.py` & `plot-antenna-1.4/setup.py`

 * *Files identical despite different names*

### Comparing `plot-antenna-1.3/test/test_plot.py` & `plot-antenna-1.4/test/test_plot.py`

 * *Files identical despite different names*

