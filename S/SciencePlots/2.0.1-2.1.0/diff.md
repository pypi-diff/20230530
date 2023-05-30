# Comparing `tmp/SciencePlots-2.0.1.tar.gz` & `tmp/SciencePlots-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SciencePlots-2.0.1.tar", last modified: Sat Dec  3 18:44:50 2022, max compression
+gzip compressed data, was "SciencePlots-2.1.0.tar", last modified: Tue May 30 13:07:56 2023, max compression
```

## Comparing `SciencePlots-2.0.1.tar` & `SciencePlots-2.1.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2022-12-03 18:44:50.713887 SciencePlots-2.0.1/
--rw-rw-rw-   0        0        0     1088 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/LICENSE
--rw-rw-rw-   0        0        0       25 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    10973 2022-12-03 18:44:50.713887 SciencePlots-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    10415 2022-11-28 20:35:20.000000 SciencePlots-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-12-03 18:44:50.546957 SciencePlots-2.0.1/SciencePlots.egg-info/
--rw-rw-rw-   0        0        0    10973 2022-12-03 18:44:50.000000 SciencePlots-2.0.1/SciencePlots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1286 2022-12-03 18:44:50.000000 SciencePlots-2.0.1/SciencePlots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-03 18:44:50.000000 SciencePlots-2.0.1/SciencePlots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-12-03 18:44:50.000000 SciencePlots-2.0.1/SciencePlots.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-12-03 18:44:50.000000 SciencePlots-2.0.1/SciencePlots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       57 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2022-12-03 18:44:50.555961 SciencePlots-2.0.1/scienceplots/
--rw-rw-rw-   0        0        0      767 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-03 18:44:50.574935 SciencePlots-2.0.1/scienceplots/styles/
-drwxrwxrwx   0        0        0        0 2022-12-03 18:44:50.630712 SciencePlots-2.0.1/scienceplots/styles/color/
--rw-rw-rw-   0        0        0      232 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/color/bright.mplstyle
--rw-rw-rw-   0        0        0      199 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/color/high-contrast.mplstyle
--rw-rw-rw-   0        0        0      241 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/color/high-vis.mplstyle
--rw-rw-rw-   0        0        0      251 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/color/light.mplstyle
--rw-rw-rw-   0        0        0      261 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/color/muted.mplstyle
--rw-rw-rw-   0        0        0      139 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/color/retro.mplstyle
--rw-rw-rw-   0        0        0      205 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/color/std-colors.mplstyle
--rw-rw-rw-   0        0        0      233 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/color/vibrant.mplstyle
-drwxrwxrwx   0        0        0        0 2022-12-03 18:44:50.644926 SciencePlots-2.0.1/scienceplots/styles/journals/
--rw-rw-rw-   0        0        0      408 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/journals/ieee.mplstyle
--rw-rw-rw-   0        0        0      937 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/journals/nature.mplstyle
-drwxrwxrwx   0        0        0        0 2022-12-03 18:44:50.710914 SciencePlots-2.0.1/scienceplots/styles/misc/
--rw-rw-rw-   0        0        0      149 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/misc/cjk-jp-font.mplstyle
--rw-rw-rw-   0        0        0      147 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/misc/cjk-kr-font.mplstyle
--rw-rw-rw-   0        0        0      159 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/misc/cjk-sc-font.mplstyle
--rw-rw-rw-   0        0        0      160 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/misc/cjk-tc-font.mplstyle
--rw-rw-rw-   0        0        0      287 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/misc/grid.mplstyle
--rw-rw-rw-   0        0        0      389 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/misc/latex-sans.mplstyle
--rw-rw-rw-   0        0        0       43 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/misc/no-latex.mplstyle
--rw-rw-rw-   0        0        0      133 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/misc/pgf.mplstyle
--rw-rw-rw-   0        0        0      200 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/misc/russian-font.mplstyle
--rw-rw-rw-   0        0        0      374 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/misc/sans.mplstyle
--rw-rw-rw-   0        0        0      227 2022-11-28 20:35:20.000000 SciencePlots-2.0.1/scienceplots/styles/misc/turkish-font.mplstyle
--rw-rw-rw-   0        0        0      679 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/notebook.mplstyle
--rw-rw-rw-   0        0        0      340 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/scatter.mplstyle
--rw-rw-rw-   0        0        0     1158 2022-11-07 00:58:29.000000 SciencePlots-2.0.1/scienceplots/styles/science.mplstyle
--rw-rw-rw-   0        0        0       42 2022-12-03 18:44:50.714891 SciencePlots-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1318 2022-12-03 18:42:02.000000 SciencePlots-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:07:56.460801 SciencePlots-2.1.0/
+-rw-rw-rw-   0        0        0     1088 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-05-30 13:03:42.000000 SciencePlots-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11037 2023-05-30 13:07:56.459689 SciencePlots-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10415 2023-05-28 18:29:03.000000 SciencePlots-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 13:07:56.394768 SciencePlots-2.1.0/SciencePlots.egg-info/
+-rw-rw-rw-   0        0        0    11037 2023-05-30 13:07:56.000000 SciencePlots-2.1.0/SciencePlots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1316 2023-05-30 13:07:56.000000 SciencePlots-2.1.0/SciencePlots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 13:07:56.000000 SciencePlots-2.1.0/SciencePlots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-30 13:07:56.000000 SciencePlots-2.1.0/SciencePlots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-30 13:07:56.000000 SciencePlots-2.1.0/SciencePlots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       57 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-30 13:07:56.396683 SciencePlots-2.1.0/scienceplots/
+-rw-rw-rw-   0        0        0      984 2023-04-05 10:26:33.000000 SciencePlots-2.1.0/scienceplots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:07:56.405685 SciencePlots-2.1.0/scienceplots/styles/
+drwxrwxrwx   0        0        0        0 2023-05-30 13:07:56.425684 SciencePlots-2.1.0/scienceplots/styles/color/
+-rw-rw-rw-   0        0        0      232 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/color/bright.mplstyle
+-rw-rw-rw-   0        0        0      199 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/color/high-contrast.mplstyle
+-rw-rw-rw-   0        0        0      241 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/color/high-vis.mplstyle
+-rw-rw-rw-   0        0        0      251 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/color/light.mplstyle
+-rw-rw-rw-   0        0        0      261 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/color/muted.mplstyle
+-rw-rw-rw-   0        0        0      139 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/color/retro.mplstyle
+-rw-rw-rw-   0        0        0      205 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/color/std-colors.mplstyle
+-rw-rw-rw-   0        0        0      233 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/color/vibrant.mplstyle
+drwxrwxrwx   0        0        0        0 2023-05-30 13:07:56.429683 SciencePlots-2.1.0/scienceplots/styles/journals/
+-rw-rw-rw-   0        0        0      487 2023-05-30 08:54:33.000000 SciencePlots-2.1.0/scienceplots/styles/journals/ieee.mplstyle
+-rw-rw-rw-   0        0        0      937 2023-05-30 09:09:41.000000 SciencePlots-2.1.0/scienceplots/styles/journals/nature.mplstyle
+drwxrwxrwx   0        0        0        0 2023-05-30 13:07:56.445685 SciencePlots-2.1.0/scienceplots/styles/languages/
+-rw-rw-rw-   0        0        0      149 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/languages/cjk-jp-font.mplstyle
+-rw-rw-rw-   0        0        0      147 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/languages/cjk-kr-font.mplstyle
+-rw-rw-rw-   0        0        0      159 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/languages/cjk-sc-font.mplstyle
+-rw-rw-rw-   0        0        0      160 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/languages/cjk-tc-font.mplstyle
+-rw-rw-rw-   0        0        0      200 2023-05-30 09:09:50.000000 SciencePlots-2.1.0/scienceplots/styles/languages/russian-font.mplstyle
+-rw-rw-rw-   0        0        0      227 2023-05-30 09:09:50.000000 SciencePlots-2.1.0/scienceplots/styles/languages/turkish-font.mplstyle
+drwxrwxrwx   0        0        0        0 2023-05-30 13:07:56.456687 SciencePlots-2.1.0/scienceplots/styles/misc/
+-rw-rw-rw-   0        0        0      287 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/misc/grid.mplstyle
+-rw-rw-rw-   0        0        0      389 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/misc/latex-sans.mplstyle
+-rw-rw-rw-   0        0        0       43 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/misc/no-latex.mplstyle
+-rw-rw-rw-   0        0        0      133 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/misc/pgf.mplstyle
+-rw-rw-rw-   0        0        0      374 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/misc/sans.mplstyle
+-rw-rw-rw-   0        0        0      679 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/notebook.mplstyle
+-rw-rw-rw-   0        0        0      340 2022-11-07 00:58:29.000000 SciencePlots-2.1.0/scienceplots/styles/scatter.mplstyle
+-rw-rw-rw-   0        0        0     1220 2023-05-30 08:54:33.000000 SciencePlots-2.1.0/scienceplots/styles/science.mplstyle
+-rw-rw-rw-   0        0        0       42 2023-05-30 13:07:56.460801 SciencePlots-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1394 2023-05-30 10:57:58.000000 SciencePlots-2.1.0/setup.py
```

### Comparing `SciencePlots-2.0.1/LICENSE` & `SciencePlots-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SciencePlots-2.0.1/PKG-INFO` & `SciencePlots-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: SciencePlots
-Version: 2.0.1
+Version: 2.1.0
 Summary: Format Matplotlib for scientific plotting
 Home-page: https://github.com/garrettj403/SciencePlots/
 Author: John Garrett
 Author-email: garrettj403@gmail.com
+Maintainer: Echedey Luis
+Maintainer-email: echelual@gmail.com
 License: MIT
 Keywords: matplotlib-style-sheets,matplotlib-figures,scientific-papers,thesis-template,matplotlib-styles,python
 Classifier: Framework :: Matplotlib
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `SciencePlots-2.0.1/README.md` & `SciencePlots-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `SciencePlots-2.0.1/SciencePlots.egg-info/PKG-INFO` & `SciencePlots-2.1.0/SciencePlots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: SciencePlots
-Version: 2.0.1
+Version: 2.1.0
 Summary: Format Matplotlib for scientific plotting
 Home-page: https://github.com/garrettj403/SciencePlots/
 Author: John Garrett
 Author-email: garrettj403@gmail.com
+Maintainer: Echedey Luis
+Maintainer-email: echelual@gmail.com
 License: MIT
 Keywords: matplotlib-style-sheets,matplotlib-figures,scientific-papers,thesis-template,matplotlib-styles,python
 Classifier: Framework :: Matplotlib
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `SciencePlots-2.0.1/SciencePlots.egg-info/SOURCES.txt` & `SciencePlots-2.1.0/SciencePlots.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 scienceplots/styles/color/light.mplstyle
 scienceplots/styles/color/muted.mplstyle
 scienceplots/styles/color/retro.mplstyle
 scienceplots/styles/color/std-colors.mplstyle
 scienceplots/styles/color/vibrant.mplstyle
 scienceplots/styles/journals/ieee.mplstyle
 scienceplots/styles/journals/nature.mplstyle
-scienceplots/styles/misc/cjk-jp-font.mplstyle
-scienceplots/styles/misc/cjk-kr-font.mplstyle
-scienceplots/styles/misc/cjk-sc-font.mplstyle
-scienceplots/styles/misc/cjk-tc-font.mplstyle
+scienceplots/styles/languages/cjk-jp-font.mplstyle
+scienceplots/styles/languages/cjk-kr-font.mplstyle
+scienceplots/styles/languages/cjk-sc-font.mplstyle
+scienceplots/styles/languages/cjk-tc-font.mplstyle
+scienceplots/styles/languages/russian-font.mplstyle
+scienceplots/styles/languages/turkish-font.mplstyle
 scienceplots/styles/misc/grid.mplstyle
 scienceplots/styles/misc/latex-sans.mplstyle
 scienceplots/styles/misc/no-latex.mplstyle
 scienceplots/styles/misc/pgf.mplstyle
-scienceplots/styles/misc/russian-font.mplstyle
-scienceplots/styles/misc/sans.mplstyle
-scienceplots/styles/misc/turkish-font.mplstyle
+scienceplots/styles/misc/sans.mplstyle
```

### Comparing `SciencePlots-2.0.1/scienceplots/__init__.py` & `SciencePlots-2.1.0/scienceplots/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from os import listdir
 from os.path import isdir, join
 
 import matplotlib.pyplot as plt
 
-import pkg_resources
+import scienceplots
 
 # register the included stylesheet in the matplotlib style library
-# TODO: migrate to importlib_resources when possible
-data_path = pkg_resources.resource_filename('scienceplots', 'styles/')
-stylesheets = plt.style.core.read_style_directory(data_path) # Reads styles in /styles
+scienceplots_path = scienceplots.__path__[0]
+styles_path = join(scienceplots_path, 'styles')
+
+# Reads styles in /styles
+stylesheets = plt.style.core.read_style_directory(styles_path)
 # Reads styles in /styles subfolders
-for inode in listdir(data_path):
-    new_data_path = join(data_path, inode)
+for inode in listdir(styles_path):
+    new_data_path = join(styles_path, inode)
     if isdir(new_data_path):
         new_stylesheets = plt.style.core.read_style_directory(new_data_path)
         stylesheets.update(new_stylesheets)
+
 # Update dictionary of styles
 plt.style.core.update_nested_dict(plt.style.library, stylesheets)
+# Update `plt.style.available`, copy-paste from:
+# https://github.com/matplotlib/matplotlib/blob/a170539a421623bb2967a45a24bb7926e2feb542/lib/matplotlib/style/core.py#L266
+plt.style.core.available[:] = sorted(plt.style.library.keys())
```

### Comparing `SciencePlots-2.0.1/scienceplots/styles/journals/nature.mplstyle` & `SciencePlots-2.1.0/scienceplots/styles/journals/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `SciencePlots-2.0.1/scienceplots/styles/notebook.mplstyle` & `SciencePlots-2.1.0/scienceplots/styles/notebook.mplstyle`

 * *Files identical despite different names*

### Comparing `SciencePlots-2.0.1/scienceplots/styles/science.mplstyle` & `SciencePlots-2.1.0/scienceplots/styles/science.mplstyle`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 legend.frameon : False
 
 # Always save as 'tight'
 savefig.bbox : tight
 savefig.pad_inches : 0.05
 
 # Use serif fonts
-# font.serif : Times
+font.serif : cmr10, Computer Modern Serif, DejaVu Serif
 font.family : serif
-mathtext.fontset : dejavuserif
+axes.formatter.use_mathtext : True
+mathtext.fontset : cm
 
 # Use LaTeX for math formatting
 text.usetex : True
 text.latex.preamble : \usepackage{amsmath} \usepackage{amssymb}
```

### Comparing `SciencePlots-2.0.1/setup.py` & `SciencePlots-2.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 # Get description from README
 root = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(root, 'README.md'), 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='SciencePlots',
-    version='2.0.1',
+    version='2.1.0',
     author="John Garrett",
     author_email="garrettj403@gmail.com",
+    maintainer="Echedey Luis",
+    maintainer_email="echelual@gmail.com",
     description="Format Matplotlib for scientific plotting",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="MIT",
     url="https://github.com/garrettj403/SciencePlots/",
 
     install_requires=['matplotlib'],
```

