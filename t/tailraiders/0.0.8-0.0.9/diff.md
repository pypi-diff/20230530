# Comparing `tmp/tailraiders-0.0.8.tar.gz` & `tmp/tailraiders-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailraiders-0.0.8.tar", last modified: Mon May 29 14:05:52 2023, max compression
+gzip compressed data, was "tailraiders-0.0.9.tar", last modified: Tue May 30 09:23:52 2023, max compression
```

## Comparing `tailraiders-0.0.8.tar` & `tailraiders-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.072926 tailraiders-0.0.8/
--rw-rw-rw-   0        0        0     1087 2023-05-29 12:00:40.000000 tailraiders-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 tailraiders-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      875 2023-05-29 14:05:52.071926 tailraiders-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      592 2023-05-29 13:52:37.000000 tailraiders-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-29 14:05:52.072926 tailraiders-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      649 2023-05-29 13:56:02.000000 tailraiders-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.024768 tailraiders-0.0.8/tailraiders/
--rw-rw-rw-   0        0        0     1066 2023-05-29 13:46:05.000000 tailraiders-0.0.8/tailraiders/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.046000 tailraiders-0.0.8/tailraiders/boaboa/
--rw-rw-rw-   0        0        0      142 2023-05-29 13:21:30.000000 tailraiders-0.0.8/tailraiders/boaboa/__init__.py
--rw-rw-rw-   0        0        0     2556 2023-05-29 13:46:50.000000 tailraiders-0.0.8/tailraiders/boaboa/doc.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.048203 tailraiders-0.0.8/tailraiders/bugtrapper/
--rw-rw-rw-   0        0        0       54 2023-05-29 13:21:39.000000 tailraiders-0.0.8/tailraiders/bugtrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.052832 tailraiders-0.0.8/tailraiders/gajalaka/
--rw-rw-rw-   0        0        0      134 2023-05-29 13:22:06.000000 tailraiders-0.0.8/tailraiders/gajalaka/__init__.py
--rw-rw-rw-   0        0        0     6313 2023-05-29 13:47:35.000000 tailraiders-0.0.8/tailraiders/gajalaka/plots.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.055832 tailraiders-0.0.8/tailraiders/plunderer/
--rw-rw-rw-   0        0        0       53 2023-05-29 13:30:09.000000 tailraiders-0.0.8/tailraiders/plunderer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.066364 tailraiders-0.0.8/tailraiders/protector/
--rw-rw-rw-   0        0        0      235 2023-05-29 13:44:08.000000 tailraiders-0.0.8/tailraiders/protector/__init__.py
--rw-rw-rw-   0        0        0     3789 2023-05-29 13:47:59.000000 tailraiders-0.0.8/tailraiders/protector/nan.py
--rw-rw-rw-   0        0        0     5395 2023-05-29 13:51:30.000000 tailraiders-0.0.8/tailraiders/protector/prep.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.068364 tailraiders-0.0.8/tailraiders/trouper/
--rw-rw-rw-   0        0        0      149 2023-05-29 13:44:18.000000 tailraiders-0.0.8/tailraiders/trouper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:05:52.042748 tailraiders-0.0.8/tailraiders.egg-info/
--rw-rw-rw-   0        0        0      875 2023-05-29 14:05:51.000000 tailraiders-0.0.8/tailraiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-05-29 14:05:51.000000 tailraiders-0.0.8/tailraiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 14:05:51.000000 tailraiders-0.0.8/tailraiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-05-29 14:05:51.000000 tailraiders-0.0.8/tailraiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-29 14:05:51.000000 tailraiders-0.0.8/tailraiders.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.958047 tailraiders-0.0.9/
+-rw-rw-rw-   0        0        0     1087 2023-05-29 12:00:40.000000 tailraiders-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 tailraiders-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      949 2023-05-30 09:23:52.958047 tailraiders-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2023-05-30 09:20:26.000000 tailraiders-0.0.9/README.md
+-rw-rw-rw-   0        0        0      229 2023-05-30 09:23:52.962996 tailraiders-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      649 2023-05-30 09:18:37.000000 tailraiders-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.866858 tailraiders-0.0.9/tailraiders/
+-rw-rw-rw-   0        0        0     1066 2023-05-30 09:12:44.000000 tailraiders-0.0.9/tailraiders/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.928845 tailraiders-0.0.9/tailraiders/boaboa/
+-rw-rw-rw-   0        0        0      142 2023-05-29 13:21:30.000000 tailraiders-0.0.9/tailraiders/boaboa/__init__.py
+-rw-rw-rw-   0        0        0     2556 2023-05-29 13:46:50.000000 tailraiders-0.0.9/tailraiders/boaboa/doc.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.931926 tailraiders-0.0.9/tailraiders/bugtrapper/
+-rw-rw-rw-   0        0        0       52 2023-05-30 09:17:49.000000 tailraiders-0.0.9/tailraiders/bugtrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.937396 tailraiders-0.0.9/tailraiders/gajalaka/
+-rw-rw-rw-   0        0        0      134 2023-05-29 13:22:06.000000 tailraiders-0.0.9/tailraiders/gajalaka/__init__.py
+-rw-rw-rw-   0        0        0     7733 2023-05-30 09:07:48.000000 tailraiders-0.0.9/tailraiders/gajalaka/plots.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.940909 tailraiders-0.0.9/tailraiders/plunderer/
+-rw-rw-rw-   0        0        0       51 2023-05-30 09:17:42.000000 tailraiders-0.0.9/tailraiders/plunderer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.951809 tailraiders-0.0.9/tailraiders/protector/
+-rw-rw-rw-   0        0        0      235 2023-05-29 13:44:08.000000 tailraiders-0.0.9/tailraiders/protector/__init__.py
+-rw-rw-rw-   0        0        0     4895 2023-05-30 08:53:12.000000 tailraiders-0.0.9/tailraiders/protector/nan.py
+-rw-rw-rw-   0        0        0     6072 2023-05-30 09:06:57.000000 tailraiders-0.0.9/tailraiders/protector/prep.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.954190 tailraiders-0.0.9/tailraiders/trouper/
+-rw-rw-rw-   0        0        0       41 2023-05-30 09:17:34.000000 tailraiders-0.0.9/tailraiders/trouper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.922294 tailraiders-0.0.9/tailraiders.egg-info/
+-rw-rw-rw-   0        0        0      949 2023-05-30 09:23:51.000000 tailraiders-0.0.9/tailraiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2023-05-30 09:23:52.000000 tailraiders-0.0.9/tailraiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 09:23:51.000000 tailraiders-0.0.9/tailraiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-05-30 09:23:51.000000 tailraiders-0.0.9/tailraiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-30 09:23:52.000000 tailraiders-0.0.9/tailraiders.egg-info/top_level.txt
```

### Comparing `tailraiders-0.0.8/LICENSE` & `tailraiders-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tailraiders-0.0.8/PKG-INFO` & `tailraiders-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailraiders
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for making Data Science easier
 Author: Busse Heemskerk
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,13 +14,14 @@
 
 ## Installation
 You can install the package by using the following code:
 ```
 pip install tailraiders
 ```
 
-## New additions: Version 0.0.8
-- Nan now has a function renamed: df_from_file is now use_file
-- tailraiders.protector has the class Outliers, for checking skewness and dealing w outliers using IQR
-- All files now follow pep8 accordingly
+## New additions: Version 0.0.9
+- Docstrings are fully updated, also the classes now have docstrings
+- The __init__ from MeltPlot has been removed due to being unnecessary
+- Added setup.cfg to make the F401 errors in __init__.py files no longer show up
+- Currently removed troupers functionality, due to errors
```

### Comparing `tailraiders-0.0.8/setup.py` & `tailraiders-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     author = 'Busse Heemskerk',
     description = 'A package for making Data Science easier',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     name = 'tailraiders',
-    version = '0.0.8',
+    version = '0.0.9',
     packages = find_packages(include = ['tailraiders', 'tailraiders.*']),
     install_requires = ['pandas>=1.0',
                         'numpy>=1.0',
                         'matplotlib>=2.2.3',
                         'seaborn>=0.9.0',
                         'sklearn>=1.0.0'],
     python_requires = '>=2.7, !=3.0.*, !=3.1.*'
```

### Comparing `tailraiders-0.0.8/tailraiders/__init__.py` & `tailraiders-0.0.9/tailraiders/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 """
 Tailraiders
 =======================================
 
 The tailraiders package is made to help with general Data Sciency stuff.
 """
 
+# Making it so you can, for certain parts, use from tailraiders import _blank_
+from tailraiders.boaboa.doc import docstring
+from tailraiders.gajalaka.plots import Plot, MeltPlot
+from tailraiders.protector.nan import Nan
+from tailraiders.protector.prep import Outliers
+
 # Checking if dependencies are installed, the dependencies
 # of my libary are stored in the dependency_module value
 dependency_module = ['pandas',
                      'numpy',
                      'matplotlib',
                      'seaborn',
                      'sklearn']
@@ -18,13 +24,7 @@
     # Try to import modules
     try:
         __import__(module)
     # Raise an error when it fails, telling them to install the failed module
     except ImportError:
         raise ImportError(f"The required package {module} \
                             was not found. Please install it.")
-
-# Making it so you can, for certain parts, use from tailraiders import _blank_
-from tailraiders.boaboa.doc import docstring
-from tailraiders.gajalaka.plots import Plot, MeltPlot
-from tailraiders.protector.nan import Nan
-from tailraiders.protector.prep import Outliers
```

### Comparing `tailraiders-0.0.8/tailraiders/boaboa/doc.py` & `tailraiders-0.0.9/tailraiders/boaboa/doc.py`

 * *Files identical despite different names*

### Comparing `tailraiders-0.0.8/tailraiders/gajalaka/plots.py` & `tailraiders-0.0.9/tailraiders/gajalaka/plots.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,80 @@
 import seaborn as sns
 import matplotlib.pyplot as plt
 
 
 class Plot:
-    """ Code for making catplots and relplots """
+    """
+    A class to make graphs that have a unified format
+
+    Attributes:
+    --------------------
+    PALETTE : str
+        The base palette given to the graphs
+
+    HEIGHT : int
+        The height of every graph
+
+    ASPECT : int
+        The aspect of every graph
+
+    df : pandas.DataFrame
+        The dataframe you use to make the graphs
+
+    xlim_low : int or float (default = None)
+        The lower limit of the x-axis of the graph
+
+    xlim_high : int or float (default = None)
+        The upper limit of the x-axis of the graph
+
+    Methods:
+    --------------------
+    cat(self, x, y, hue=None, kind='bar')
+        A function to make a catplot, based on the dataframe used for Plot
+
+    rel(self, x, y, hue=None, kind='scatter')
+        A function to make a relplot, based on the dataframe used for Plot
+    """
+
     # Adding standard values for heigt, aspect and palette
     PALETTE = "plasma"
     HEIGHT = 4
     ASPECT = 3
 
     def __init__(self, df, xlim_low=None, xlim_high=None):
+        """
+        The initiator, sets the df as data and sets
+        the x-axis limits
+
+        Parameters:
+        --------------------
+        df : pandas.DataFrame
+            The dataframe you use to make the graphs
+
+        xlim_low : int or float (default = None)
+            The lower limit of the x-axis of the graph
+
+        xlim_high : int or float (default = None)
+            The upper limit of the x-axis of the graph
+        """
+
         self.data = df
         self._df = self.data
         self.xlim_low = xlim_low
         self.xlim_high = xlim_high
         sns.set_style('darkgrid')
 
     def cat(self, x, y, hue=None, kind='bar'):
         """
         A function to make a catplot, based on the dataframe used for Plot
 
         Parameters:
-        --------------
+        --------------------
         self :
-            The given name of the class
+            The instance of this class
 
         x : str
             Column name for x parameter
 
         y : str
             Column name for y parameter
 
@@ -35,15 +82,15 @@
             A column name for differentiating per category
 
         kind : str (default = 'bar')
             The kind of plot you want to make, options are:
                 strip, swarm, box, violin, boxen, point, bar and count
 
         Returns:
-        --------------
+        --------------------
         None :
             Instead it shows the plot for which the parameters are given
         """
 
         # try-except so it will show all columns if you use the wrong column
         try:
             # making the catplot using seaborn and defining certain attributes
@@ -58,17 +105,17 @@
                              a column name. Check {[*self._df.columns]}")
 
     def rel(self, x, y, hue=None, kind='scatter'):
         """
         A function to make a relplot, based on the dataframe used for Plot
 
         Parameters:
-        --------------
+        --------------------
         self :
-            The given name of the class
+            The instance of this class
 
         x : str
             Column name for x parameter
 
         y : str
             Column name for y parameter
 
@@ -76,15 +123,15 @@
             A column name for differentiating per category
 
         kind : str (default = 'bar')
             The kind of plot you want to make, options are:
                 strip, swarm, box, violin, boxen, point, bar and count
 
         Returns:
-        --------------
+        --------------------
         None :
             Instead it shows the plot for which the parameters are given
         """
 
         # try-except so it will show all columns if you use the wrong column
         try:
             # making the relplot using seaborn and defining certain attributes
@@ -96,39 +143,43 @@
             plt.show()
         except ValueError:
             raise ValueError(f"Make sure x, y and hue are \
                              a column name. Check {[*self._df.columns]}")
 
 
 class MeltPlot(Plot):
-    """ A child-class that uses a melted dataframe to make visualisations """
-    def __init__(self, data, xlim_low=None, xlim_high=None):
-        Plot.__init__(self, data, xlim_low, xlim_high)
+    """
+    A child-class to make graphs that have a unified format,
+    inheriting attributes from its parentclass Plot.
+    This class makes use of .melt to make the data.
+    To make use of melt, cat needs a list on the x-axis
+    and rel needs a list on the y-axis
+    """
 
     def cat(self, x, y, kind='bar'):
         """
         A function to make a catplot, based on the dataframe used for Plot
 
         Parameters:
-        --------------
+        --------------------
         self :
-            The given name of the class
+            The instance of this class
 
-        x : str
+        x : str or list
             Column name for x parameter
 
         y : str
             Column name for y parameter
 
         kind : str (default = 'bar')
             The kind of plot you want to make, options are:
                 strip, swarm, box, violin, boxen, point, bar and count
 
         Returns:
-        --------------
+        --------------------
         None :
             Instead it shows the plot for which the parameters are given
         """
 
         # try-except so it will show all columns if you use the wrong column
         try:
             # if-statement so that the function will work
@@ -146,30 +197,30 @@
                            a column name. Check {[*self._df.columns]}")
 
     def rel(self, x, y, kind='scatter'):
         """
         A function to make a relplot, based on the dataframe used for Plot
 
         Parameters:
-        --------------
+        --------------------
         self :
-            The given name of the class
+            The instance of this class
 
         x : str
             Column name for x parameter
 
-        y : str
+        y : str or list
             Column name for y parameter
 
         kind : str (default = 'scatter')
             The kind of plot you want to make, options are:
                 strip, swarm, box, violin, boxen, point, bar and count
 
         Returns:
-        --------------
+        --------------------
         None :
             Instead it shows the plot for which the parameters are given
         """
 
         # try-except so it will show all columns if you use the wrong column
         try:
             # if-statement so that the function will work
```

### Comparing `tailraiders-0.0.8/tailraiders/protector/nan.py` & `tailraiders-0.0.9/tailraiders/protector/nan.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,55 @@
 import pandas as pd
 
 
 class Nan:
-    """ Checks for NaN values and manipulate them """
+    """
+    A class used for working with missing values.
+
+    Attributes:
+    --------------------
+    df : pandas.DataFrame
+        A pandas dataframe where you want to look
+        at the missing values and work with them
+
+    Methods:
+    --------------------
+    __init__(self, df)
+        The initiator, making a dataframe containing
+        the amount of missing values per column
+
+    drop_cols(self, th=20)
+        Drops columns based on the given threshold
+
+    fill_na(self, col, group, stat='mean')
+        Fills dataframe column based on
+        a given group and method
+
+    drop_na(self, axis=0)
+        Drops columns based on the given axis
+
+    use_file(cls, file_path)
+        A function to immediately convert files to work for Nan
+    """
+
     def __init__(self, df):
+        """
+        The initiator, making a dataframe containing
+        the amount of missing values per column
+
+        Parameters:
+        --------------------
+        self :
+            The instance of this class
+
+        df : pandas.DataFrame
+            A pandas dataframe where you want to look
+            at the missing values and work with them
+        """
+
         self.df = df
         self.missing = df.isna().sum().to_frame()
         self.values = df.count().to_frame()
         self.rows = self.missing + self.values
         self.perc = round(self.missing / self.rows * 100, 2)
         self.dfnan = pd.concat([self.missing, self.values,
                                 self.rows, self.perc], axis=1)
@@ -15,24 +57,24 @@
                               'rows without nan', 'perc nan']
 
     def drop_cols(self, th=20):
         """
         Drops columns based on a given threshold
 
         Parameters:
-        ---------------
+        --------------------
         self :
-            The given name of the class
+            The instance of this class
 
         th : int (default = 20)
             The percentage threshold of when
             columns should be dropped
 
         Returns:
-        ----------------
+        --------------------
         None :
             It makes it so that self.df is now edited
             to no longer has the dropped columns
         """
 
         # making a temp df to see what columns go over the threshold
         self.nan_df = self.dfnan[self.dfnan['perc nan'] > th]
@@ -43,33 +85,33 @@
 
         # dropping the columns in the list
         self.df = self.df.drop(dropcols, axis=1)
         self.__init__(self.df)
 
     def fill_na(self, col, group, stat='mean'):
         """
-        Fills dataframe columns based on
+        Fills dataframe column based on
         a given group and method
 
         Parameters:
-        --------------
+        --------------------
         self :
-            The given name of the class
+            The instance of this class
 
         col : str
             The column name that will be filled
 
         group : str
             Column name that will be used to group by
 
         stat : str (default = 'mean')
             The stat on how people will be grouped
 
         Returns:
-        ----------------
+        --------------------
         None :
             It makes it so that self.df is now edited
             to no longer have the dropped columns
         """
 
         # using fillna to fill the given column with
         # given groupby column using the given method
@@ -79,24 +121,24 @@
         self.__init__(self.df)
 
     def drop_na(self, axis=0):
         """
         Drops columns based on the given axis
 
         Parameters:
-        ---------------
+        --------------------
         self :
-            The given name of the class
+            The instance of this class
 
         axis : int (default = 0)
             Bool value, either 0 or 1. 0 is
             for rows and 1 is for columns
 
         Returns:
-        ----------------
+        --------------------
         None :
             It makes it so that self.df is now edited
             to no longer have the dropped rows or columns
         """
 
         # dropna to drop rows or columns, based on given axis
         self.df = self.df.dropna(axis=axis)
@@ -106,15 +148,15 @@
     def use_file(cls, file_path):
         """
         A function to immediately convert files to be used for Nan
 
         Parameters
         --------------------
         cls :
-            The class it is in (will not be filled in when using the function)
+            The object resembling this class
 
         file_path : str
             The file_path to the file containing the data you want to use
 
         returns:
         --------------------
         cls(df) : pandas.Dataframe
```

### Comparing `tailraiders-0.0.8/tailraiders/protector/prep.py` & `tailraiders-0.0.9/tailraiders/protector/prep.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,44 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 
 class Outliers:
-    """ A class to analyse and deal with potential outliers """
+    """
+    A class to handle the outliers in a dataframe
+
+    Attributes:
+    --------------------
+    df : pandas.DataFrame
+        The dataframe of which you want to look for outliers
+
+    Methods:
+    --------------------
+    check_skew(self, column, th=0.5)
+        This function checks the skewness of a given
+        column from the dataframe passed in the class
+
+    def check_outliers(self, column, th=1.5, remove=False)
+        This function checks a column for outliers if
+        there is a normal distribution and possibly removes them.
+        Checking the outliers is based on using the Inter Quartile Range.
+    """
+
     def __init__(self, df):
+        """
+        The initiator, makes the passed df into a class df
+        """
+
         self.df = df
 
     def check_skew(self, column, th=0.5):
         """
         This function checks the skewness of a given
-        column from the dataframe given to the class
+        column from the dataframe passed in the class
 
         Parameters:
         --------------------
         self :
             The given name of the class
 
         column : str
```

### Comparing `tailraiders-0.0.8/tailraiders.egg-info/PKG-INFO` & `tailraiders-0.0.9/tailraiders.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailraiders
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package for making Data Science easier
 Author: Busse Heemskerk
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,13 +14,14 @@
 
 ## Installation
 You can install the package by using the following code:
 ```
 pip install tailraiders
 ```
 
-## New additions: Version 0.0.8
-- Nan now has a function renamed: df_from_file is now use_file
-- tailraiders.protector has the class Outliers, for checking skewness and dealing w outliers using IQR
-- All files now follow pep8 accordingly
+## New additions: Version 0.0.9
+- Docstrings are fully updated, also the classes now have docstrings
+- The __init__ from MeltPlot has been removed due to being unnecessary
+- Added setup.cfg to make the F401 errors in __init__.py files no longer show up
+- Currently removed troupers functionality, due to errors
```

### Comparing `tailraiders-0.0.8/tailraiders.egg-info/SOURCES.txt` & `tailraiders-0.0.9/tailraiders.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+setup.cfg
 setup.py
 tailraiders/__init__.py
 tailraiders.egg-info/PKG-INFO
 tailraiders.egg-info/SOURCES.txt
 tailraiders.egg-info/dependency_links.txt
 tailraiders.egg-info/requires.txt
 tailraiders.egg-info/top_level.txt
```

