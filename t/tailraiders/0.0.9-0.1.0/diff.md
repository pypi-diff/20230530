# Comparing `tmp/tailraiders-0.0.9.tar.gz` & `tmp/tailraiders-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailraiders-0.0.9.tar", last modified: Tue May 30 09:23:52 2023, max compression
+gzip compressed data, was "tailraiders-0.1.0.tar", last modified: Tue May 30 09:55:41 2023, max compression
```

## Comparing `tailraiders-0.0.9.tar` & `tailraiders-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.958047 tailraiders-0.0.9/
--rw-rw-rw-   0        0        0     1087 2023-05-29 12:00:40.000000 tailraiders-0.0.9/LICENSE
--rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 tailraiders-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0      949 2023-05-30 09:23:52.958047 tailraiders-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      666 2023-05-30 09:20:26.000000 tailraiders-0.0.9/README.md
--rw-rw-rw-   0        0        0      229 2023-05-30 09:23:52.962996 tailraiders-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      649 2023-05-30 09:18:37.000000 tailraiders-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.866858 tailraiders-0.0.9/tailraiders/
--rw-rw-rw-   0        0        0     1066 2023-05-30 09:12:44.000000 tailraiders-0.0.9/tailraiders/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.928845 tailraiders-0.0.9/tailraiders/boaboa/
--rw-rw-rw-   0        0        0      142 2023-05-29 13:21:30.000000 tailraiders-0.0.9/tailraiders/boaboa/__init__.py
--rw-rw-rw-   0        0        0     2556 2023-05-29 13:46:50.000000 tailraiders-0.0.9/tailraiders/boaboa/doc.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.931926 tailraiders-0.0.9/tailraiders/bugtrapper/
--rw-rw-rw-   0        0        0       52 2023-05-30 09:17:49.000000 tailraiders-0.0.9/tailraiders/bugtrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.937396 tailraiders-0.0.9/tailraiders/gajalaka/
--rw-rw-rw-   0        0        0      134 2023-05-29 13:22:06.000000 tailraiders-0.0.9/tailraiders/gajalaka/__init__.py
--rw-rw-rw-   0        0        0     7733 2023-05-30 09:07:48.000000 tailraiders-0.0.9/tailraiders/gajalaka/plots.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.940909 tailraiders-0.0.9/tailraiders/plunderer/
--rw-rw-rw-   0        0        0       51 2023-05-30 09:17:42.000000 tailraiders-0.0.9/tailraiders/plunderer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.951809 tailraiders-0.0.9/tailraiders/protector/
--rw-rw-rw-   0        0        0      235 2023-05-29 13:44:08.000000 tailraiders-0.0.9/tailraiders/protector/__init__.py
--rw-rw-rw-   0        0        0     4895 2023-05-30 08:53:12.000000 tailraiders-0.0.9/tailraiders/protector/nan.py
--rw-rw-rw-   0        0        0     6072 2023-05-30 09:06:57.000000 tailraiders-0.0.9/tailraiders/protector/prep.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.954190 tailraiders-0.0.9/tailraiders/trouper/
--rw-rw-rw-   0        0        0       41 2023-05-30 09:17:34.000000 tailraiders-0.0.9/tailraiders/trouper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:23:52.922294 tailraiders-0.0.9/tailraiders.egg-info/
--rw-rw-rw-   0        0        0      949 2023-05-30 09:23:51.000000 tailraiders-0.0.9/tailraiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      560 2023-05-30 09:23:52.000000 tailraiders-0.0.9/tailraiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 09:23:51.000000 tailraiders-0.0.9/tailraiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-05-30 09:23:51.000000 tailraiders-0.0.9/tailraiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-30 09:23:52.000000 tailraiders-0.0.9/tailraiders.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 09:55:41.547661 tailraiders-0.1.0/
+-rw-rw-rw-   0        0        0     1087 2023-05-29 12:00:40.000000 tailraiders-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 tailraiders-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      817 2023-05-30 09:55:41.548668 tailraiders-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-05-30 09:54:30.000000 tailraiders-0.1.0/README.md
+-rw-rw-rw-   0        0        0      229 2023-05-30 09:55:41.559190 tailraiders-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      606 2023-05-30 09:53:36.000000 tailraiders-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:55:41.470289 tailraiders-0.1.0/tailraiders/
+-rw-rw-rw-   0        0        0     1033 2023-05-30 09:27:42.000000 tailraiders-0.1.0/tailraiders/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:55:41.520810 tailraiders-0.1.0/tailraiders/boaboa/
+-rw-rw-rw-   0        0        0      142 2023-05-29 13:21:30.000000 tailraiders-0.1.0/tailraiders/boaboa/__init__.py
+-rw-rw-rw-   0        0        0     2557 2023-05-30 09:53:21.000000 tailraiders-0.1.0/tailraiders/boaboa/doc.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:55:41.524836 tailraiders-0.1.0/tailraiders/bugtrapper/
+-rw-rw-rw-   0        0        0       52 2023-05-30 09:17:49.000000 tailraiders-0.1.0/tailraiders/bugtrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:55:41.530393 tailraiders-0.1.0/tailraiders/gajalaka/
+-rw-rw-rw-   0        0        0      134 2023-05-29 13:22:06.000000 tailraiders-0.1.0/tailraiders/gajalaka/__init__.py
+-rw-rw-rw-   0        0        0     7735 2023-05-30 09:52:48.000000 tailraiders-0.1.0/tailraiders/gajalaka/plots.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:55:41.532995 tailraiders-0.1.0/tailraiders/plunderer/
+-rw-rw-rw-   0        0        0       51 2023-05-30 09:17:42.000000 tailraiders-0.1.0/tailraiders/plunderer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:55:41.542697 tailraiders-0.1.0/tailraiders/protector/
+-rw-rw-rw-   0        0        0      235 2023-05-29 13:44:08.000000 tailraiders-0.1.0/tailraiders/protector/__init__.py
+-rw-rw-rw-   0        0        0     4895 2023-05-30 08:53:12.000000 tailraiders-0.1.0/tailraiders/protector/nan.py
+-rw-rw-rw-   0        0        0     6122 2023-05-30 09:49:08.000000 tailraiders-0.1.0/tailraiders/protector/prep.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:55:41.545258 tailraiders-0.1.0/tailraiders/trouper/
+-rw-rw-rw-   0        0        0       41 2023-05-30 09:17:34.000000 tailraiders-0.1.0/tailraiders/trouper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:55:41.515787 tailraiders-0.1.0/tailraiders.egg-info/
+-rw-rw-rw-   0        0        0      817 2023-05-30 09:55:39.000000 tailraiders-0.1.0/tailraiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2023-05-30 09:55:41.000000 tailraiders-0.1.0/tailraiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 09:55:39.000000 tailraiders-0.1.0/tailraiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-30 09:55:40.000000 tailraiders-0.1.0/tailraiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-30 09:55:40.000000 tailraiders-0.1.0/tailraiders.egg-info/top_level.txt
```

### Comparing `tailraiders-0.0.9/LICENSE` & `tailraiders-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tailraiders-0.0.9/PKG-INFO` & `tailraiders-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: tailraiders
-Version: 0.0.9
+Version: 0.1.0
 Summary: A package for making Data Science easier
 Author: Busse Heemskerk
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tailraiders
-Tailraiders is a package currently **under development**. It is meant to be used for school and potentially later for Data Science. Modeled after the Tailraiders Alliance Factions, all subpackages are named after those.
+Tailraiders is a package currently still **under development**. It is meant to be used for school and potentially later for Data Science. Modeled after the Tailraiders Alliance Factions, all subpackages are named after those.
 
 ## Installation
 You can install the package by using the following code:
 ```
 pip install tailraiders
 ```
 
-## New additions: Version 0.0.9
-- Docstrings are fully updated, also the classes now have docstrings
-- The __init__ from MeltPlot has been removed due to being unnecessary
-- Added setup.cfg to make the F401 errors in __init__.py files no longer show up
-- Currently removed troupers functionality, due to errors
+## New additions: Version 0.1.0
+- Errors and prints are now displayed properly when running the code
+- First more major release, due to this being a now fullfilled assignment
```

### Comparing `tailraiders-0.0.9/README.md` & `tailraiders-0.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Tailraiders
-Tailraiders is a package currently **under development**. It is meant to be used for school and potentially later for Data Science. Modeled after the Tailraiders Alliance Factions, all subpackages are named after those.
+Tailraiders is a package currently still **under development**. It is meant to be used for school and potentially later for Data Science. Modeled after the Tailraiders Alliance Factions, all subpackages are named after those.
 
 ## Installation
 You can install the package by using the following code:
 ```
 pip install tailraiders
 ```
 
-## New additions: Version 0.0.9
-- Docstrings are fully updated, also the classes now have docstrings
-- The __init__ from MeltPlot has been removed due to being unnecessary
-- Added setup.cfg to make the F401 errors in __init__.py files no longer show up
-- Currently removed troupers functionality, due to errors
+## New additions: Version 0.1.0
+- Errors and prints are now displayed properly when running the code
+- First more major release, due to this being a now fullfilled assignment
```

### Comparing `tailraiders-0.0.9/setup.py` & `tailraiders-0.1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 setup(
     author = 'Busse Heemskerk',
     description = 'A package for making Data Science easier',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     name = 'tailraiders',
-    version = '0.0.9',
+    version = '0.1.0',
     packages = find_packages(include = ['tailraiders', 'tailraiders.*']),
     install_requires = ['pandas>=1.0',
                         'numpy>=1.0',
                         'matplotlib>=2.2.3',
-                        'seaborn>=0.9.0',
-                        'sklearn>=1.0.0'],
+                        'seaborn>=0.9.0'],
     python_requires = '>=2.7, !=3.0.*, !=3.1.*'
     )
```

### Comparing `tailraiders-0.0.9/tailraiders/__init__.py` & `tailraiders-0.1.0/tailraiders/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 from tailraiders.protector.prep import Outliers
 
 # Checking if dependencies are installed, the dependencies
 # of my libary are stored in the dependency_module value
 dependency_module = ['pandas',
                      'numpy',
                      'matplotlib',
-                     'seaborn',
-                     'sklearn']
+                     'seaborn']
 
 # For-loop to check for modules
 for module in dependency_module:
     # Try to import modules
     try:
         __import__(module)
     # Raise an error when it fails, telling them to install the failed module
```

### Comparing `tailraiders-0.0.9/tailraiders/boaboa/doc.py` & `tailraiders-0.1.0/tailraiders/boaboa/doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,10 +52,10 @@
         doc += f'    {return_name} : {return_type}\n        {return_expl}\n'
         doc += '    """'
 
         return print(doc)
 
     # Raises an error when amount_args != an integer
     else:
-        raise ValueError(f'The amount of arguments {amount_args} \
-                         is not an integer, please refrain from \
-                         trying non-integers')
+        raise ValueError("The amount of arguments {amount_args} "
+                         "is not an integer, please refrain from "
+                         "trying non-integers")
```

### Comparing `tailraiders-0.0.9/tailraiders/gajalaka/plots.py` & `tailraiders-0.1.0/tailraiders/gajalaka/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,16 +189,16 @@
             else:
                 # making a melted df to use for Plot.cat
                 self._df = self.data[x + [y]].melt(id_vars=y)
                 hue = 'variable'
                 x = 'value'
                 Plot.cat(self, x, y, hue, kind)
         except KeyError:
-            raise KeyError(f"Make sure x, y and hue are \
-                           a column name. Check {[*self._df.columns]}")
+            raise KeyError("Make sure x, y and hue are "
+                           f"a column name. Check {[*self._df.columns]}")
 
     def rel(self, x, y, kind='scatter'):
         """
         A function to make a relplot, based on the dataframe used for Plot
 
         Parameters:
         --------------------
@@ -230,9 +230,9 @@
             else:
                 # making a melted df to use for Plot.rel
                 self._df = self.data[[x] + y].melt(id_vars=x)
                 hue = 'variable'
                 x = 'value'
                 Plot.rel(self, x, y, hue, kind)
         except KeyError:
-            raise KeyError(f"Make sure x, y and hue are \
-                           a column name. Check {[*self._df.columns]}")
+            raise KeyError("Make sure x, y and hue are "
+                           f"a column name. Check {[*self._df.columns]}")
```

### Comparing `tailraiders-0.0.9/tailraiders/protector/nan.py` & `tailraiders-0.1.0/tailraiders/protector/nan.py`

 * *Files identical despite different names*

### Comparing `tailraiders-0.0.9/tailraiders/protector/prep.py` & `tailraiders-0.1.0/tailraiders/protector/prep.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         --------------------
         None :
             Instead returns two print statements and a graph
             detailing and showing the distribution of the column
         """
 
         # If-statement to check for int or float
-        if isinstance(self.df[column], (int, float)):
+        if all(isinstance(value, (int, float)) for value in self.df[column]):
             # Checking the skewness of the given column
             skewness = self.df[column].skew()
 
             # if-statement for the type of skewness
             if abs(skewness) <= th:
                 skewness_type = "Symmetric"
             elif skewness > 0:
@@ -78,17 +78,17 @@
             plt.xlabel("Values")
             plt.ylabel("Frequency")
             plt.title(f"Distribution of {column}")
             plt.show()
 
         # raising an error when column isnt int or float
         else:
-            raise ValueError(f'The column {column} is not \
-                             interger or float, so skewness \
-                             cannot be calculated')
+            raise ValueError(f"The column {column} is not "
+                             "interger or float, so skewness "
+                             "cannot be calculated")
 
     def check_outliers(self, column, th=1.5, remove=False):
         """
         This function checks a column for outliers if
         there is a normal distribution and possibly removes them.
         Checking the outliers is based on using the Inter Quartile Range.
 
@@ -119,23 +119,23 @@
             # Process a single column
             columns = [column]
         elif isinstance(column, list) and \
                 all(isinstance(col, str) for col in column):
             # Process each column in the list
             columns = column
         else:
-            raise ValueError("The column parameter must be \
-                             a string or a list of strings.")
+            raise ValueError("The column parameter must be "
+                             "a string or a list of strings.")
 
         # Create a list to store outliers for each column
         skipped_columns = []
 
         for col in columns:
             # If-statement to check for int or float
-            if isinstance(self.df[col], (int, float)):
+            if all(isinstance(value, (int, float)) for value in self.df[col]):
                 # Making the quartile ranges
                 q1 = np.percentile(self.df[col], 25)
                 q3 = np.percentile(self.df[col], 75)
                 iqr = q3 - q1
 
                 # Making the upper and lower bounds for the values
                 # to see if they are considered an outlier
@@ -163,11 +163,11 @@
             # Append the col into the skipped_columns list
             else:
                 skipped_columns.append(col)
                 continue
 
         # If columns are skipped, print the columns that were skipped
         if len(skipped_columns) > 0:
-            print(f"The following columns were skipped \
-                    due to non-numeric values: {skipped_columns}")
+            print("The following columns were skipped "
+                  f"due to non-numeric values: {skipped_columns}")
 
         return self.df
```

### Comparing `tailraiders-0.0.9/tailraiders.egg-info/PKG-INFO` & `tailraiders-0.1.0/tailraiders.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: tailraiders
-Version: 0.0.9
+Version: 0.1.0
 Summary: A package for making Data Science easier
 Author: Busse Heemskerk
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tailraiders
-Tailraiders is a package currently **under development**. It is meant to be used for school and potentially later for Data Science. Modeled after the Tailraiders Alliance Factions, all subpackages are named after those.
+Tailraiders is a package currently still **under development**. It is meant to be used for school and potentially later for Data Science. Modeled after the Tailraiders Alliance Factions, all subpackages are named after those.
 
 ## Installation
 You can install the package by using the following code:
 ```
 pip install tailraiders
 ```
 
-## New additions: Version 0.0.9
-- Docstrings are fully updated, also the classes now have docstrings
-- The __init__ from MeltPlot has been removed due to being unnecessary
-- Added setup.cfg to make the F401 errors in __init__.py files no longer show up
-- Currently removed troupers functionality, due to errors
+## New additions: Version 0.1.0
+- Errors and prints are now displayed properly when running the code
+- First more major release, due to this being a now fullfilled assignment
```

### Comparing `tailraiders-0.0.9/tailraiders.egg-info/SOURCES.txt` & `tailraiders-0.1.0/tailraiders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

