# Comparing `tmp/RecruitmentCurveFitting-1.0.1-py2.py3-none-any.whl.zip` & `tmp/RecruitmentCurveFitting-1.1.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 105806 bytes, number of entries: 12
+Zip file size: 106261 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    35821 b- defN 23-May-27 05:45 RecruitmentCurveFitting/COPYING
--rw-r--r--  2.0 unx    18188 b- defN 23-May-27 23:59 RecruitmentCurveFitting/CurveFitting.py
+-rw-r--r--  2.0 unx    18750 b- defN 23-May-30 15:02 RecruitmentCurveFitting/CurveFitting.py
 -rw-r--r--  2.0 unx    28108 b- defN 23-May-27 05:02 RecruitmentCurveFitting/RecruitmentCurves.py
--rw-r--r--  2.0 unx     4153 b- defN 23-May-27 23:59 RecruitmentCurveFitting/__init__.py
--rw-r--r--  2.0 unx     6695 b- defN 23-May-27 23:59 RecruitmentCurveFitting/__main__.py
+-rw-r--r--  2.0 unx     4153 b- defN 23-May-30 15:02 RecruitmentCurveFitting/__init__.py
+-rw-r--r--  2.0 unx     7760 b- defN 23-May-30 15:02 RecruitmentCurveFitting/__main__.py
 -rw-r--r--  2.0 unx     1491 b- defN 23-May-27 02:43 RecruitmentCurveFitting/example-data1.txt
 -rw-r--r--  2.0 unx     2291 b- defN 23-May-27 02:24 RecruitmentCurveFitting/example-data2.txt
 -rw-r--r--  2.0 unx   208425 b- defN 23-May-27 02:24 RecruitmentCurveFitting/example-waveforms.csv
--rw-r--r--  2.0 unx     2602 b- defN 23-May-27 23:59 RecruitmentCurveFitting-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-27 23:59 RecruitmentCurveFitting-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-May-27 23:59 RecruitmentCurveFitting-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1135 b- defN 23-May-27 23:59 RecruitmentCurveFitting-1.0.1.dist-info/RECORD
-12 files, 309043 bytes uncompressed, 103866 bytes compressed:  66.4%
+-rw-r--r--  2.0 unx     2602 b- defN 23-May-30 15:02 RecruitmentCurveFitting-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-30 15:02 RecruitmentCurveFitting-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-May-30 15:02 RecruitmentCurveFitting-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1135 b- defN 23-May-30 15:02 RecruitmentCurveFitting-1.1.0.dist-info/RECORD
+12 files, 310670 bytes uncompressed, 104321 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: RecruitmentCurveFitting/example-data2.txt
 Comment: 
 
 Filename: RecruitmentCurveFitting/example-waveforms.csv
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.0.1.dist-info/METADATA
+Filename: RecruitmentCurveFitting-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.0.1.dist-info/WHEEL
+Filename: RecruitmentCurveFitting-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.0.1.dist-info/top_level.txt
+Filename: RecruitmentCurveFitting-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.0.1.dist-info/RECORD
+Filename: RecruitmentCurveFitting-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## RecruitmentCurveFitting/CurveFitting.py

```diff
@@ -307,22 +307,25 @@
 				if param.isFixed: param.finalValue = fullParamDict[ param.name ]
 			atMin = [ param.name for param in self._FREEPARAMS if param.isAtMin ]
 			atMax = [ param.name for param in self._FREEPARAMS if param.isAtMax ]
 			if atMin: print( '#    hit lower bound: %s' % ', '.join( atMin ) )
 			if atMax: print( '#    hit upper bound: %s' % ', '.join( atMax ) )
 		return self
 			
-	def Plot( self, data=True, guess=False, fit=True, markX=None, markY=None, title=False, grid=None, xlabel=None, ylabel=None, hold='auto', figure=None, axes=None, **kwargs ):
+	def Plot( self, data=True, guess=False, fit=True, markX=None, markY=None, title=False, grid=None, xlabel=None, ylabel=None, hold='auto', figure=None, axes=None, xlim=None, ylim=None, **kwargs ):
 		import matplotlib.pyplot as plt
 		axes = plt.gcf() if axes is None else plt.figure( axes ) if isinstance( axes, int ) else axes
 		if isinstance( axes, plt.Figure ): axes = axes.gca()
 		
 		figure = axes.figure
 		self.axes = axes
-		xlim = self.x.min(), self.x.max()
+		if xlim is None: xlim = self.x.min(), self.x.max()
+		elif isinstance( xlim, ( float, int ) ) or len( xlim ) == 1:
+			xlim = numpy.asarray( xlim ).ravel()[ 0 ]
+			xlim = [ xlim, self.x.max() ] if abs( xlim - self.x.min() ) < abs( xlim - self.x.max() ) else [ self.x.min(), xlim ]
 		x = numpy.linspace( xlim[ 0 ], xlim[ -1 ], 200 )
 		if hold in [ None, 'auto' ]: hold = not data
 		if not hold: axes.cla()
 		hGuess = hFit = hData = None
 		if self.excuses:
 			if not hold: axes.set( xticks=[], yticks=[] )
 			axes.text( 0.5, 0.5, '\n'.join( self.excuses ), transform=axes.transAxes, ha='center', va='center' )
@@ -379,23 +382,29 @@
 			for x in markX:
 				#if not min( xlim ) <= x <= max( xlim ): continue
 				axes.plot( [ x, x ], [ 0.0, 1.0 ], transform=axes.get_xaxis_transform(), **props )
 		if markY is not None:
 			markY = [ maxY if y == 'max' else y  for y in ( markY.flat if isinstance( markY, numpy.ndarray ) else markY ) ]
 			markY = numpy.asarray( markY ).ravel().tolist()
 			props = dict(); props.update( kwargs, marker=None, linestyle=':' )	
-			#ylim = axes.get_ylim()
 			for y in markY:
-				#if not min( ylim ) <= y <= max( ylim ): continue
 				axes.plot( [ 0.0, 1.0 ], [ y, y ], transform=axes.get_yaxis_transform(), **props )
 		
 		if grid is not None: axes.grid( grid )
 		if xlabel is not None: axes.set_xlabel( xlabel )
 		if ylabel is not None: axes.set_ylabel( ylabel )
-		if title: axes.set_title( title if isinstance( title, str ) else self.Describe( ' ', wrap=45 ), fontsize=7, fontweight='bold' )
+		if xlim is not None: axes.set_xlim( xlim )
+		if ylim is not None:
+			if isinstance( ylim, ( float, int ) ) or len( ylim ) == 1:
+				auto_ylim = sorted( axes.get_ylim() )
+				ylim = [ ylim, auto_ylim[ 1 ] ] if abs( ylim - auto_ylim[ 0 ] ) < abs( ylim - auto_ylim[ 1 ] ) else [ auto_ylim[ 0 ], ylim ]
+			axes.set_ylim( ylim )
+		if title:
+			if not isinstance( title, str ): title = '@DEFAULT@'
+			axes.set_title( title.replace( '@DEFAULT@', self.Describe( ' ', wrap=45 ) ), fontsize=7, fontweight='bold' )
 		return self
 		
 	def _mpl_disconnect( self ):	
 		axes = getattr( self, 'axes', None )
 		connection = getattr( self, 'mpl_connect_id', None )
 		if axes is not None and connection is not None:
 			try: axes.figure.canvas.mpl_disconnect( connection )
```

## RecruitmentCurveFitting/__init__.py

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-__version__ = '1.0.1'
+__version__ = '1.1.0'
 
 # $BEGIN_RECRUITMENTCURVEFITTING_LICENSE$
 # 
 # This file is part of the RecruitmentCurveFitting project, a Python
 # package for fitting sigmoid and bell-shaped functions to EMG
 # recruitment-curve measurements.
 #
```

## RecruitmentCurveFitting/__main__.py

```diff
@@ -26,30 +26,48 @@
 
 """
 Use the RecruitmentCurveFitting module from the command-line
 to fit both an M-wave and an H-reflex recruitment curve from
 one or more text files.
 """
 
+import os
+import re
+import ast
+import sys
+import glob
 import argparse
+
+def OneOrTwoNumbers( s ):
+	seq = ast.literal_eval( s.strip( ' [](),' ) + ',' )
+	try: x, = seq
+	except: x = a, b = seq
+	return x
+		
+
 class HelpFormatter( argparse.RawDescriptionHelpFormatter ): pass
 #class HelpFormatter( argparse.RawDescriptionHelpFormatter, argparse.ArgumentDefaultsHelpFormatter ): pass
 parser = argparse.ArgumentParser( description=__doc__, formatter_class=HelpFormatter, prog='python -m RecruitmentCurveFitting', )
 parser.add_argument(         "filenames",    metavar='FILENAME',    nargs='*', help='one or more text files to load (use a dash to denote stdin)' )
-parser.add_argument( "-t", "--threshold",    metavar='MTHRESHOLD',  default=0.1, type=float, help='unscaled proportion of Mmax (between 0 and 1) that is considered "threshold" for the M-wave curve' )
-parser.add_argument( "-s", "--saveas",       metavar='PDFFILENAME', default='', help='name of pdf file in which to save figures' )
+parser.add_argument( "-s", "--saveas",       metavar='PDFFILENAME', default='', help='name of pdf file in which to save figures (one per page)' )
 parser.add_argument( "-p", "--plot",         action='store_true',   help='whether to show figures on-screen' )
 parser.add_argument( "-g", "--grid",         action='store_true',   help='whether to use a grid for the plot' )
 parser.add_argument( "-x", "--xlabel",       metavar='XLABEL',      default='Stimulation Intensity (mA)', help='x-axis label text for the plot' )
 parser.add_argument( "-y", "--ylabel",       metavar='YLABEL',      default='Response ($\\mu$V)', help='y-axis label text for the plot' )
+parser.add_argument(       "--title",        metavar='TITLE',       default=None, help='override automatically-generated plot titles' )
+parser.add_argument(       "--xlim",         metavar='XMIN,XMAX',   default=None, type=OneOrTwoNumbers, help='x-axis limits for the plot' )
+parser.add_argument(       "--ylim",         metavar='YMIN,YMAX',   default=None, type=OneOrTwoNumbers, help='y-axis limits for the plot' )
+parser.add_argument(       "--mark-mmax",    action='store_true',   help='whether to mark M_max' )
+parser.add_argument(       "--mark-hmax",    action='store_true',   help='whether to mark H_max' )
+parser.add_argument( "-t", "--threshold",    metavar='MTHRESHOLD',  default=0, type=float, help='unscaled proportion of Mmax (between 0 and 1) to mark as "threshold" for the M-wave curve (set to 0 to leave it unmarked)' )
 parser.add_argument(       "--unpack-examples", action='store_true', help='write example files to the current directory (do not overwrite) and quit' )
 parser.add_argument(       "--help-module",  action='store_true', help='display the main package docstring' )
 opts = parser.parse_args()
 
-import os, re, ast, sys, glob
+
 import numpy
 
 import RecruitmentCurveFitting
 from RecruitmentCurveFitting import *
 
 if opts.unpack_examples:
 	UnpackExamples()
@@ -120,15 +138,17 @@
 		'Hmax' : hMax,
 		'HmaxStim' : hMaxStim,
 	} )
 	conditionDict.update( { 'M_' + k : v for k, v in m.ResolveParameters( asDict=True ).items() } )
 	conditionDict.update( { 'H_' + k : v for k, v in h.ResolveParameters( asDict=True ).items() } )
 	print( '%r,\n' % conditionDict )
 	if opts.plot or opts.saveas:
-		m.Plot( axes=eachCondition, markX=mThresholdStim, markY=mMax )
-		h.Plot( axes=eachCondition, markX='max', markY='max', hold=True, title=True, grid=opts.grid, xlabel=opts.xlabel, ylabel=opts.ylabel )
+		if opts.title is None: opts.title = '@DEFAULT@'
+		else: opts.title = ast.literal_eval( '"""' + opts.title + '"""' )
+		m.Plot( axes=eachCondition, markX=mThresholdStim, markY=mMax if opts.mark_mmax else None, xlim=opts.xlim )
+		h.Plot( axes=eachCondition, markX='max' if opts.mark_hmax else None, markY='max' if opts.mark_hmax else None, hold=True, title=opts.title, grid=opts.grid, xlabel=opts.xlabel, ylabel=opts.ylabel, xlim=opts.xlim, ylim=opts.ylim )
 print( ']' )
 if opts.saveas:
 	opts.saveas = os.path.realpath( os.path.expanduser( opts.saveas ) )
 	print( '# saving %d figure%s to %s' % ( len( conditions ), '' if len( conditions ) == 1 else 's',  opts.saveas ) )
 	SavePDF( opts.saveas, figures=conditions )
 if opts.plot and 'IPython' not in sys.modules: import matplotlib; matplotlib.pyplot.show()
```

## Comparing `RecruitmentCurveFitting-1.0.1.dist-info/METADATA` & `RecruitmentCurveFitting-1.1.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RecruitmentCurveFitting
-Version: 1.0.1
+Version: 1.1.0
 Summary: A package for fitting sigmoid and bell-shaped functions to EMG recruitment-curve measurements
 Home-page: UNKNOWN
 Author: Jeremy Hill
 Author-email: jezhill@gmail.com
 License: GPL v3+
 Platform: UNKNOWN
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, <4
```

## Comparing `RecruitmentCurveFitting-1.0.1.dist-info/RECORD` & `RecruitmentCurveFitting-1.1.0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 RecruitmentCurveFitting/COPYING,sha256=Czg9WmPaZE9ijZnDOXbqZIftiaqlnwsyV5kt6sEXHms,35821
-RecruitmentCurveFitting/CurveFitting.py,sha256=2QrG4bXN-4TIZiNEQcW1U3EQbXxuhMC2620CBUzZbFE,18188
+RecruitmentCurveFitting/CurveFitting.py,sha256=80RF2UuoP9KUl-pydCIwa_FHD9k8-J7OFvefHWRfL2A,18750
 RecruitmentCurveFitting/RecruitmentCurves.py,sha256=Glpy6G3ttJ1gBnIv0ITVPr4MtSTLslWauWRZbqOFK8g,28108
-RecruitmentCurveFitting/__init__.py,sha256=ZiUIZ1Vn1r9p0Fm7jooQ3T8a89xWdAVd4Dav6iUFnUU,4153
-RecruitmentCurveFitting/__main__.py,sha256=I71DOcLNvMHohrnGZQjaMPLSD9zdiFRqikEvV3JUCpI,6695
+RecruitmentCurveFitting/__init__.py,sha256=peOEQXA8V176MhvCWwFqLxkv4coU7H70YOjM5Lc3RCo,4153
+RecruitmentCurveFitting/__main__.py,sha256=Itk6SIM0iEb1UY_RsRH9yNHAxMjz-GGFuLe8yhjNivg,7760
 RecruitmentCurveFitting/example-data1.txt,sha256=FeaYwnAMGemLQKM9Kj1IPi_3fey7gyY9SLOJYttZcXc,1491
 RecruitmentCurveFitting/example-data2.txt,sha256=SBv6zHDxt1YOhylfZSMMHSCsDNwL1brHpTgAdH8esvg,2291
 RecruitmentCurveFitting/example-waveforms.csv,sha256=eWF7HtChJAv5uHfiQ1Pg__l-d9eYKtGWr8PlYp7-kis,208425
-RecruitmentCurveFitting-1.0.1.dist-info/METADATA,sha256=Kpsp9DWWQv1EU5TA8jB3_trvq_L46nZQ5kXS-iTIW1s,2602
-RecruitmentCurveFitting-1.0.1.dist-info/WHEEL,sha256=h_aVn5OB2IERUjMbi2pucmR_zzWJtk303YXvhh60NJ8,110
-RecruitmentCurveFitting-1.0.1.dist-info/top_level.txt,sha256=GaYHShtnr9zJ_unau13fDnezLMr3kyCH0-KQN_Go6WM,24
-RecruitmentCurveFitting-1.0.1.dist-info/RECORD,,
+RecruitmentCurveFitting-1.1.0.dist-info/METADATA,sha256=msRPJiVYu-EJisdOWMJKTEw-OYeN2dr6VwcsObCbrmE,2602
+RecruitmentCurveFitting-1.1.0.dist-info/WHEEL,sha256=h_aVn5OB2IERUjMbi2pucmR_zzWJtk303YXvhh60NJ8,110
+RecruitmentCurveFitting-1.1.0.dist-info/top_level.txt,sha256=GaYHShtnr9zJ_unau13fDnezLMr3kyCH0-KQN_Go6WM,24
+RecruitmentCurveFitting-1.1.0.dist-info/RECORD,,
```

