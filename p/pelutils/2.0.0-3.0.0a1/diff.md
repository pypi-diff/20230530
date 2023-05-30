# Comparing `tmp/pelutils-2.0.0.tar.gz` & `tmp/pelutils-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelutils-2.0.0.tar", last modified: Sun Dec 25 17:25:28 2022, max compression
+gzip compressed data, was "pelutils-3.0.0a1.tar", last modified: Tue May 30 02:06:46 2023, max compression
```

## Comparing `pelutils-2.0.0.tar` & `pelutils-3.0.0a1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 17:25:28.054826 pelutils-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-25 17:25:26.000000 pelutils-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2022-12-25 17:25:28.054826 pelutils-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12016 2022-12-25 17:25:26.000000 pelutils-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 17:25:28.054826 pelutils-2.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-25 17:25:26.000000 pelutils-2.0.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2022-12-25 17:25:26.000000 pelutils-2.0.0/examples/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 17:25:28.054826 pelutils-2.0.0/examples/ds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-25 17:25:26.000000 pelutils-2.0.0/examples/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2022-12-25 17:25:26.000000 pelutils-2.0.0/examples/ds/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 17:25:28.054826 pelutils-2.0.0/pelutils/
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2022-12-25 17:25:26.000000 pelutils-2.0.0/pelutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-25 17:25:26.000000 pelutils-2.0.0/pelutils/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 17:25:28.054826 pelutils-2.0.0/pelutils/_c/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2022-12-25 17:25:26.000000 pelutils-2.0.0/pelutils/_c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2022-12-25 17:25:26.000000 pelutils-2.0.0/pelutils/_c/ds.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 17:25:28.054826 pelutils-2.0.0/pelutils/_c/hashmap.c/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2022-12-25 17:25:27.000000 pelutils-2.0.0/pelutils/_c/hashmap.c/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29789 2022-12-25 17:25:27.000000 pelutils-2.0.0/pelutils/_c/hashmap.c/hashmap.c
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2022-12-25 17:25:27.000000 pelutils-2.0.0/pelutils/_c/hashmap.c/hashmap.h
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2022-12-25 17:25:26.000000 pelutils-2.0.0/pelutils/datastorage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 17:25:28.054826 pelutils-2.0.0/pelutils/ds/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2022-12-25 17:25:26.000000 pelutils-2.0.0/pelutils/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2022-12-25 17:25:26.000000 pelutils-2.0.0/pelutils/ds/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2022-12-25 17:25:26.000000 pelutils-2.0.0/pelutils/ds/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2022-12-25 17:25:26.000000 pelutils-2.0.0/pelutils/ds/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2022-12-25 17:25:26.000000 pelutils-2.0.0/pelutils/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2022-12-25 17:25:26.000000 pelutils-2.0.0/pelutils/jsonl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 17:25:28.054826 pelutils-2.0.0/pelutils/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2022-12-25 17:25:26.000000 pelutils-2.0.0/pelutils/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2022-12-25 17:25:26.000000 pelutils-2.0.0/pelutils/logging/support.py
--rw-r--r--   0 runner    (1001) docker     (123)    19853 2022-12-25 17:25:26.000000 pelutils-2.0.0/pelutils/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2022-12-25 17:25:26.000000 pelutils-2.0.0/pelutils/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10221 2022-12-25 17:25:26.000000 pelutils-2.0.0/pelutils/ticktock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-25 17:25:28.054826 pelutils-2.0.0/pelutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2022-12-25 17:25:28.000000 pelutils-2.0.0/pelutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      757 2022-12-25 17:25:28.000000 pelutils-2.0.0/pelutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-25 17:25:28.000000 pelutils-2.0.0/pelutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-25 17:25:28.000000 pelutils-2.0.0/pelutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      327 2022-12-25 17:25:28.000000 pelutils-2.0.0/pelutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-25 17:25:28.000000 pelutils-2.0.0/pelutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-25 17:25:28.054826 pelutils-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2022-12-25 17:25:26.000000 pelutils-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:06:46.259553 pelutils-3.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-05-30 02:06:46.259553 pelutils-3.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:06:46.255553 pelutils-3.0.0a1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/examples/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:06:46.255553 pelutils-3.0.0a1/examples/ds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/examples/ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/examples/ds/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:06:46.255553 pelutils-3.0.0a1/pelutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/pelutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/pelutils/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:06:46.255553 pelutils-3.0.0a1/pelutils/_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/pelutils/_c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/pelutils/_c/ds.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:06:46.255553 pelutils-3.0.0a1/pelutils/_c/hashmap.c/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-30 02:06:45.000000 pelutils-3.0.0a1/pelutils/_c/hashmap.c/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29789 2023-05-30 02:06:45.000000 pelutils-3.0.0a1/pelutils/_c/hashmap.c/hashmap.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-30 02:06:45.000000 pelutils-3.0.0a1/pelutils/_c/hashmap.c/hashmap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/pelutils/datastorage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:06:46.259553 pelutils-3.0.0a1/pelutils/ds/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/pelutils/ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/pelutils/ds/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/pelutils/ds/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/pelutils/ds/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/pelutils/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/pelutils/jsonl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:06:46.259553 pelutils-3.0.0a1/pelutils/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/pelutils/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/pelutils/logging/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19853 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/pelutils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/pelutils/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/pelutils/ticktock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:06:46.255553 pelutils-3.0.0a1/pelutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-05-30 02:06:46.000000 pelutils-3.0.0a1/pelutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-30 02:06:46.000000 pelutils-3.0.0a1/pelutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 02:06:46.000000 pelutils-3.0.0a1/pelutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-30 02:06:46.000000 pelutils-3.0.0a1/pelutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-30 02:06:46.000000 pelutils-3.0.0a1/pelutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 02:06:46.000000 pelutils-3.0.0a1/pelutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 02:06:46.259553 pelutils-3.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-30 02:06:44.000000 pelutils-3.0.0a1/setup.py
```

### Comparing `pelutils-2.0.0/PKG-INFO` & `pelutils-3.0.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelutils
-Version: 2.0.0
+Version: 3.0.0a1
 Summary: Utility functions that are often useful
 Home-page: https://github.com/peleiden/pelutils
 Author: Asger Laurits Schultz, Søren Winkel Holm
 Author-email: asger.s@protonmail.com, swholm@protonmail.com
 License: BSD-3-Clause
 Download-URL: https://pypi.org/project/pelutils/
 Keywords: utility,logger,parser,profiling,plotting
@@ -13,31 +13,31 @@
 Description-Content-Type: text/markdown
 Provides-Extra: ds
 Provides-Extra: tests
 License-File: pelutils/_c/hashmap.c/LICENSE
 
 # pelutils
 
+[![pytest](https://github.com/peleiden/pelutils/actions/workflows/pytest.yml/badge.svg?branch=master)](https://github.com/peleiden/pelutils/actions/workflows/pytest.yml)
+[![Coverage Status](https://coveralls.io/repos/github/peleiden/pelutils/badge.svg?branch=master)](https://coveralls.io/github/peleiden/pelutils?branch=master)
+
 Various utilities useful for Python projects. Features include
 
 - A simple and powerful logger with colourful printing and stacktrace logging
 - Parsing for combining config files and command-line arguments - especially useful for algorithms with several parameters
 - A timer inspired by Matlab's `tic` and `toc`
 - Simple code profiler
 - An extension to the built-in `dataclass` for saving and loading data
 - Table formatting
 - Miscellaneous standalone functions - see `pelutils/__init__.py`
 - Data-science submodule with extra utilities for statistics, plotting with `matplotlib`, and machine learning using `PyTorch`
 - Linear time `unique` function in the style of `numpy.unique`
 
 `pelutils` supports Python 3.7+.
 
-[![pytest](https://github.com/peleiden/pelutils/actions/workflows/pytest.yml/badge.svg?branch=master)](https://github.com/peleiden/pelutils/actions/workflows/pytest.yml)
-[![Coverage Status](https://coveralls.io/repos/github/peleiden/pelutils/badge.svg?branch=master)](https://coveralls.io/github/peleiden/pelutils?branch=master)
-
 ## Timing and Code Profiling
 
 Simple time taker inspired by Matlab Tic, Toc, which also has profiling tooling.
 
 ```py
 # Time a task
 TT.tick()
@@ -84,43 +84,33 @@
         tt2.tick()
     time.sleep(0.01)
 ```
 
 ## Data Storage
 
 The DataStorage class is an augmentation of the dataclass that incluces save and load functionality.
-This simplifies saving data, as only save command has to be issued for all data, and it keeps type hinting when loading data compared to e.g. a dictionary.
+This simplifies saving data, as only save command has to be issued for all data, and it keeps type
+hinting when loading data compared to e.g. a dictionary.
 
-Currently works specifically with:
-
-- Numpy arrays (`numpy.ndarray`)
-- Torch tensors (`torch.Tensor`)
-- Any `json` serializable data (as determined by the `rapidjson` library)
-
-All other data is pickled.
-
-DataStorage classes must inherit from DataStorage and be annotated with `@dataclass`.
-
-It is further possible to give arguments to the class definition:
-
-- `json_name`: Name of the saved json file
-- `indent`: How many spaces to use for indenting in the json file
+Data is in general preserved exactly as-is when saved data is loaded into memory with few exceptions.
+Notably, tuples are considered json-serializble, and so will be saved to the json file and will be
+loaded as lists.
 
 Usage example:
 
 ```py
 @dataclass
-class ResultData(DataStorage, json_name="game.json", indent=4):
+class ResultData(DataStorage):
     shots: int
     goalscorers: list
     dists: np.ndarray
 
 rdata = ResultData(shots=1, goalscorers=["Max Fenger"], dists=np.ones(22)*10)
 rdata.save("max")
-# Now shots and goalscorers are saved in <pwd>/max/game.json and dists in <pwd>/max/dists.npy
+# Now shots and goalscorers are saved in <pwd>/max/ResultData.json and dists in <pwd>/max/ResultData.pkl
 
 # Then to load
 rdata = ResultData.load("max")
 print(rdata.goalscorers)  # ["Max Fenger"]
 ```
 
 ## Parsing
@@ -260,15 +250,16 @@
 a, b = np.random.randn(100), np.random.randn(100)
 r, lower_r, upper_r, p = corr_ci(a, b, alpha=0.01)
 ```
 
 ## Plotting
 
 `pelutils` provides plotting utilities based on `matplotlib`.
-Most notable is the `Figure` context class, which attempts to remedy some of the common grievances with `matplotlib`, e.g. having to remember the correct `kwargs` and `rcParams` for setting font sizes, grid line colours etc, and notably adding type hinting to `fig` and `ax` produced by `plt.subplots`.
+Most notable is the `Figure` context class, which attempts to remedy some of the common grievances with `matplotlib`,
+e.g. having to remember the correct `kwargs` and `rcParams` for setting font sizes, legend edge colour etc.
 ```py
 from pelutils.ds.plots import Figure
 
 # The following makes a plot and saves it to `plot.png`.
 # The seaborn is style is used for demonstration, but if the `style` argument
 # is not given, the default matplotlib style is used.
 # The figure and font size are also given for demonstration, but their default
@@ -278,43 +269,35 @@
     plt.scatter(x, y, label="Data")
     plt.grid()
     plt.title("Very nice plot")
 # The figure is automatically saved to `plot.png` and closed, such that
 # plt.plot can be used again from here.
 # Figure changes `matplotlib.rcParams`, but these changes are also undone
 # after the end of the `with statement`.
-
-# For more complex plots, it is also possible to access the `fig` and `ax`
-# variables usually assigned as `fig, ax = plt.subplots()`.
-# These are type hinted, so no more remembering if it is `ax.title()` or
-# `ax.set_title()`.
-with Figure("plot.png") as f:
-    f.fig  # fig available as attribute on the Figure instance
-    f.ax.set_title("Very nice plot")  # The same goes for `ax`
 ```
 
 The plotting utilies also include binning functions for creating nice histograms.
-The `get_bins` function produces bins based on a binning function, of which three are provided:
+The `histogram` function produces bins based on a binning function, of which three are provided:
 
 - `linear_binning`: Bins are spaced evenly from the lowest to the largest value of the data.
 - `log_binning`: Bins are log-spaced from the lowest to the largest value of the data, which is assumed to be positive.
 - `normal_binning`: Bins are distributed according to the distribution of the data, such there are more bins closer to the center of the data. This is useful if the data somewhat resembles a normal distribution, as the resolution will be the greatest where there is the most data.
 
 It is also possible to provide custom binning functions.
 
-`get_bins` provide both `x` and `y` coordinates, making it simple to use with argument unpacking:
+`histogram` provide both `x` and `y` coordinates, making it simple to use with argument unpacking:
 ```py
 import matplotlib.pyplot as plt
 import numpy as np
-from pelutils.ds.plots import get_bins, normal_binning
+from pelutils.ds.plots import histogram, normal_binning
 
 # Generate normally distributed data
 x = np.random.randn(100)
 # Plot distribution
-plt.plot(*get_bins(x, binning_fn=normal_binning))
+plt.plot(*histogram(x, binning_fn=normal_binning))
 ```
 
 Finally, different smoothing functions are provided.
 The two most common are `moving_avg` and `exponential_avg` which smooth the data using a moving average and exponential smoothing, respectively.
 
 The `double_moving_avg` is special in that the number of smoothed data points do not depend on the number of given data points but is instead based on a given number of samples, which allows the resulting smoothed curve to not by jagged as happens with the other smoothing functions.
 It also has two smoothness parameters, which allows a large degree of smoothness control.
```

### Comparing `pelutils-2.0.0/README.md` & `pelutils-3.0.0a1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # pelutils
 
+[![pytest](https://github.com/peleiden/pelutils/actions/workflows/pytest.yml/badge.svg?branch=master)](https://github.com/peleiden/pelutils/actions/workflows/pytest.yml)
+[![Coverage Status](https://coveralls.io/repos/github/peleiden/pelutils/badge.svg?branch=master)](https://coveralls.io/github/peleiden/pelutils?branch=master)
+
 Various utilities useful for Python projects. Features include
 
 - A simple and powerful logger with colourful printing and stacktrace logging
 - Parsing for combining config files and command-line arguments - especially useful for algorithms with several parameters
 - A timer inspired by Matlab's `tic` and `toc`
 - Simple code profiler
 - An extension to the built-in `dataclass` for saving and loading data
 - Table formatting
 - Miscellaneous standalone functions - see `pelutils/__init__.py`
 - Data-science submodule with extra utilities for statistics, plotting with `matplotlib`, and machine learning using `PyTorch`
 - Linear time `unique` function in the style of `numpy.unique`
 
 `pelutils` supports Python 3.7+.
 
-[![pytest](https://github.com/peleiden/pelutils/actions/workflows/pytest.yml/badge.svg?branch=master)](https://github.com/peleiden/pelutils/actions/workflows/pytest.yml)
-[![Coverage Status](https://coveralls.io/repos/github/peleiden/pelutils/badge.svg?branch=master)](https://coveralls.io/github/peleiden/pelutils?branch=master)
-
 ## Timing and Code Profiling
 
 Simple time taker inspired by Matlab Tic, Toc, which also has profiling tooling.
 
 ```py
 # Time a task
 TT.tick()
@@ -67,43 +67,33 @@
         tt2.tick()
     time.sleep(0.01)
 ```
 
 ## Data Storage
 
 The DataStorage class is an augmentation of the dataclass that incluces save and load functionality.
-This simplifies saving data, as only save command has to be issued for all data, and it keeps type hinting when loading data compared to e.g. a dictionary.
+This simplifies saving data, as only save command has to be issued for all data, and it keeps type
+hinting when loading data compared to e.g. a dictionary.
 
-Currently works specifically with:
-
-- Numpy arrays (`numpy.ndarray`)
-- Torch tensors (`torch.Tensor`)
-- Any `json` serializable data (as determined by the `rapidjson` library)
-
-All other data is pickled.
-
-DataStorage classes must inherit from DataStorage and be annotated with `@dataclass`.
-
-It is further possible to give arguments to the class definition:
-
-- `json_name`: Name of the saved json file
-- `indent`: How many spaces to use for indenting in the json file
+Data is in general preserved exactly as-is when saved data is loaded into memory with few exceptions.
+Notably, tuples are considered json-serializble, and so will be saved to the json file and will be
+loaded as lists.
 
 Usage example:
 
 ```py
 @dataclass
-class ResultData(DataStorage, json_name="game.json", indent=4):
+class ResultData(DataStorage):
     shots: int
     goalscorers: list
     dists: np.ndarray
 
 rdata = ResultData(shots=1, goalscorers=["Max Fenger"], dists=np.ones(22)*10)
 rdata.save("max")
-# Now shots and goalscorers are saved in <pwd>/max/game.json and dists in <pwd>/max/dists.npy
+# Now shots and goalscorers are saved in <pwd>/max/ResultData.json and dists in <pwd>/max/ResultData.pkl
 
 # Then to load
 rdata = ResultData.load("max")
 print(rdata.goalscorers)  # ["Max Fenger"]
 ```
 
 ## Parsing
@@ -243,15 +233,16 @@
 a, b = np.random.randn(100), np.random.randn(100)
 r, lower_r, upper_r, p = corr_ci(a, b, alpha=0.01)
 ```
 
 ## Plotting
 
 `pelutils` provides plotting utilities based on `matplotlib`.
-Most notable is the `Figure` context class, which attempts to remedy some of the common grievances with `matplotlib`, e.g. having to remember the correct `kwargs` and `rcParams` for setting font sizes, grid line colours etc, and notably adding type hinting to `fig` and `ax` produced by `plt.subplots`.
+Most notable is the `Figure` context class, which attempts to remedy some of the common grievances with `matplotlib`,
+e.g. having to remember the correct `kwargs` and `rcParams` for setting font sizes, legend edge colour etc.
 ```py
 from pelutils.ds.plots import Figure
 
 # The following makes a plot and saves it to `plot.png`.
 # The seaborn is style is used for demonstration, but if the `style` argument
 # is not given, the default matplotlib style is used.
 # The figure and font size are also given for demonstration, but their default
@@ -261,43 +252,35 @@
     plt.scatter(x, y, label="Data")
     plt.grid()
     plt.title("Very nice plot")
 # The figure is automatically saved to `plot.png` and closed, such that
 # plt.plot can be used again from here.
 # Figure changes `matplotlib.rcParams`, but these changes are also undone
 # after the end of the `with statement`.
-
-# For more complex plots, it is also possible to access the `fig` and `ax`
-# variables usually assigned as `fig, ax = plt.subplots()`.
-# These are type hinted, so no more remembering if it is `ax.title()` or
-# `ax.set_title()`.
-with Figure("plot.png") as f:
-    f.fig  # fig available as attribute on the Figure instance
-    f.ax.set_title("Very nice plot")  # The same goes for `ax`
 ```
 
 The plotting utilies also include binning functions for creating nice histograms.
-The `get_bins` function produces bins based on a binning function, of which three are provided:
+The `histogram` function produces bins based on a binning function, of which three are provided:
 
 - `linear_binning`: Bins are spaced evenly from the lowest to the largest value of the data.
 - `log_binning`: Bins are log-spaced from the lowest to the largest value of the data, which is assumed to be positive.
 - `normal_binning`: Bins are distributed according to the distribution of the data, such there are more bins closer to the center of the data. This is useful if the data somewhat resembles a normal distribution, as the resolution will be the greatest where there is the most data.
 
 It is also possible to provide custom binning functions.
 
-`get_bins` provide both `x` and `y` coordinates, making it simple to use with argument unpacking:
+`histogram` provide both `x` and `y` coordinates, making it simple to use with argument unpacking:
 ```py
 import matplotlib.pyplot as plt
 import numpy as np
-from pelutils.ds.plots import get_bins, normal_binning
+from pelutils.ds.plots import histogram, normal_binning
 
 # Generate normally distributed data
 x = np.random.randn(100)
 # Plot distribution
-plt.plot(*get_bins(x, binning_fn=normal_binning))
+plt.plot(*histogram(x, binning_fn=normal_binning))
 ```
 
 Finally, different smoothing functions are provided.
 The two most common are `moving_avg` and `exponential_avg` which smooth the data using a moving average and exponential smoothing, respectively.
 
 The `double_moving_avg` is special in that the number of smoothed data points do not depend on the number of given data points but is instead based on a given number of samples, which allows the resulting smoothed curve to not by jagged as happens with the other smoothing functions.
 It also has two smoothness parameters, which allows a large degree of smoothness control.
```

### Comparing `pelutils-2.0.0/examples/ds/plots.py` & `pelutils-3.0.0a1/examples/ds/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Plotting examples using pelutils.ds.plot """
 import click
 import matplotlib.pyplot as plt
 import numpy as np
 
 from pelutils.ds.plots import (
-    linear_binning, log_binning, normal_binning, get_bins,
+    linear_binning, log_binning, normal_binning, histogram,
     moving_avg, exp_moving_avg, double_moving_avg, tab_colours,
     Figure,
 )
 from pelutils.ds.distributions import norm, lognorm
 
 
 @click.command("plots-binning")
@@ -22,30 +22,30 @@
     y_log = lognorm(mu, sigma2).rvs(N)
 
     with Figure("plots-binning.png", figsize=(22, 10)):
         # Normal distribution using linear binning
         x = np.linspace(y.min(), y.max(), 100)
         plt.subplot(131)
         plt.plot(x, norm(mu, sigma2).pdf(x))
-        plt.plot(*get_bins(y, bins=bins), marker=".")
+        plt.plot(*histogram(y, bins=bins), marker=".")
         plt.title("Normal distribution\nLinear binning")
         plt.grid()
 
         # Normal distribution using normal binning
         plt.subplot(132)
         plt.plot(x, norm(mu, sigma2).pdf(x))
-        plt.plot(*get_bins(y, binning_fn=normal_binning, bins=bins), marker=".")
+        plt.plot(*histogram(y, binning_fn=normal_binning, bins=bins), marker=".")
         plt.title("Normal distribution\nNormal binning")
         plt.grid()
 
         # Log normal distribution using logarithmic binning
         x = np.logspace(np.log10(y_log.min()), np.log10(y_log.max()), 100)
         plt.subplot(133)
         plt.plot(x, lognorm(mu, sigma2).pdf(x))
-        plt.plot(*get_bins(y_log, binning_fn=log_binning, bins=bins), marker=".")
+        plt.plot(*histogram(y_log, binning_fn=log_binning, bins=bins), marker=".")
         plt.title("Log normal distribution\nLogarithmic binning")
         plt.grid()
         plt.xscale("log")
 
 @click.command("plots-moving")
 def plots_moving():
```

### Comparing `pelutils-2.0.0/pelutils/__init__.py` & `pelutils-3.0.0a1/pelutils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,24 @@
 import ctypes
 import os
 import random
 import subprocess
 import sys
 
 import cpuinfo
-import git
+try:
+    # If git is not installed, this import fails
+    import git
+    _has_git = True
+except ImportError:
+    _has_git = False
 import psutil
 import numpy as np
 try:
+    # torch is only to be installed if pelutils[ds] has been installed
     import torch
     _has_torch = True
 except:
     _has_torch = False
 
 
 _T = TypeVar("_T")
@@ -45,14 +51,16 @@
 
 def get_repo(path: str | None=None) -> tuple[str | None, str | None]:
     """
     Returns absolute path of git repository and commit SHA
     Searches for repo by searching upwards from given directory (if None: uses working dir).
     If it cannot find a repository, returns (None, None)
     """
+    if not _has_git:
+        return None, None
     if path is None:
         path = os.getcwd()
     cdir = os.path.join(path, ".")
     pdir = os.path.dirname(cdir)
     while cdir != pdir:
         cdir = pdir
         try:  # Check if repository
```

### Comparing `pelutils-2.0.0/pelutils/_c/__init__.py` & `pelutils-3.0.0a1/pelutils/_c/__init__.py`

 * *Files identical despite different names*

### Comparing `pelutils-2.0.0/pelutils/_c/ds.c` & `pelutils-3.0.0a1/pelutils/_c/ds.c`

 * *Files identical despite different names*

### Comparing `pelutils-2.0.0/pelutils/_c/hashmap.c/LICENSE` & `pelutils-3.0.0a1/pelutils/_c/hashmap.c/LICENSE`

 * *Files identical despite different names*

### Comparing `pelutils-2.0.0/pelutils/_c/hashmap.c/hashmap.c` & `pelutils-3.0.0a1/pelutils/_c/hashmap.c/hashmap.c`

 * *Files identical despite different names*

### Comparing `pelutils-2.0.0/pelutils/_c/hashmap.c/hashmap.h` & `pelutils-3.0.0a1/pelutils/_c/hashmap.c/hashmap.h`

 * *Files identical despite different names*

### Comparing `pelutils-2.0.0/pelutils/datastorage.py` & `pelutils-3.0.0a1/pelutils/datastorage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,148 +1,122 @@
 from __future__ import annotations
 from collections import defaultdict
 from typing import Optional
 import os
 import pickle
 
-import numpy as np
 import rapidjson
-try:
-    import torch
-    _has_torch = True
-except:
-    _has_torch = False
 
 
-# The special serializations that DataStorage supports.
-# datatype: tuple consisting of save function (API is save(file, data)), load function (API is load(file_obj)) and extension
-# Can be extended by user if necessary
-SERIALIZATIONS = {
-    np.ndarray: (np.save, np.load, "npy"),
-}
-if _has_torch:
-    SERIALIZATIONS[torch.Tensor] = lambda f, d: torch.save(d, f), torch.load, "pt"
-
 class DataStorage:
     """ The DataStorage class is an augmentation of the dataclass that incluces save and load functionality.
-
-    Currently works specifically with:
-    - Numpy arrays (numpy.ndarray)
-    - Torch tensors (torch.Tensor)
-    - Any json serializable type - that is, it should be savable by json.dump
-    All other data structures are pickled.
-
-    DataStorage classes must inherit from DataStorage and be annotated with `@dataclass`.
-    It is further possible to give arguments to the class definition:
-    - `json_name`: Name of the saved json file
-    - `indent`:    How many spaces to use for indenting in the json file
+    DataStorage classes must inherit from DataStorage and be annotated with `@dataclass`. Data will be saved
+    to two files: A json files for json-serializable data and a pickle file for everything else. These files
+    are by default named after the class, but it is possible to use a custom name in the save and load methods.
+    The files are only created if necessary, so for instance if all data is json-serializable, no pickle file
+    will be created.
+
+    Data is in general preserved exactly as-is when saved data is loaded into memory with few exceptions.
+    Nnotably, tuples are considered json-serializble, and so will be saved to the json file and will be
+    loaded as lists.
 
     Usage example:
     ```py
     @dataclass
-    class ResultData(DataStorage, json_name="game.json", indent=4):
+    class ResultData(DataStorage):
         shots: int
         goalscorers: list
         dists: np.ndarray
 
     rdata = ResultData(shots=1, goalscorers=["Max Fenger"], dists=np.ones(22)*10)
     rdata.save("max")
-    # Now shots and goalscorers are saved in <pwd>/max/game.json and dists in <pwd>/max/dists.npy
+    # Now shots and goalscorers are saved in <pwd>/max/ResultData.json and dists in <pwd>/max/ResultData.pkl
 
     # Then to load
     rdata = ResultData.load("max")
     print(rdata.goalscorers)  # ["Max Fenger"]
     ``` """
 
-    _pickle_ext = "pkl"
-
-    def __init_subclass__(cls, *, json_name="data.json", indent: Optional[int]=None):
-        cls._json_name  = json_name
-        cls._indent     = indent
-
     def __init__(self, *args, **kwargs):
         """ This method is overwritten class is decorated with @dataclass.
         Therefore, if this method is called, it is an error. """
         raise TypeError("DataStorage class %s must be decorated with @dataclass" % self.__class__.__name__)
 
-    def save(self, loc: str) -> list[str]:
+    @classmethod
+    def json_name(cls, save_name: Optional[str] = None):
+        return (save_name or cls.__name__) + ".json"
+
+    @classmethod
+    def pickle_name(cls, save_name: Optional[str] = None):
+        return (save_name or cls.__name__) + ".pkl"
+
+    def save(self, loc: str, save_name: Optional[str] = None, *, indent: Optional[int] = 4) -> list[str]:
         """ Saves all the fields of the instatiated data classes as either json,
-        pickle or designated serialization function.
+        pickle or designated serialization function. Use save_name to overwrite
+        default behavior of using the class name for file names. E.g. in a DataStorage
+        class named Results, the defualt saved file names would be Results.json and
+        Results.pkl. Settings save_name="gollum" would result in file names
+        Returns list of saved files.
         :param str loc: Path to directory in which to save data. """
 
         os.makedirs(loc, exist_ok=True)
 
-        # Split data by whether it should be saved using a known function or using pickle or json
-        func_serialize = defaultdict(dict)
-        to_pickle, to_json = dict(), dict()
+        to_json = dict()
+        to_pickle = dict()
+
         for key, data in self.__dict__.items():
-            for datatype in SERIALIZATIONS:
-                if isinstance(data, datatype):
-                    func_serialize[datatype][key] = data
-                    break
-            else:
-                try:
-                    # Test whether the data is json serializable by dumping it to string.
-                    rapidjson.dumps({key: data})
-                    to_json[key] = data
-                except TypeError:
-                    to_pickle[key] = data
+            try:
+                # Test whether the data is json serializable by dumping it to string.
+                rapidjson.dumps({key: data})
+                to_json[key] = data
+            except TypeError:
+                to_pickle[key] = data
 
         # Save data
         paths = list()
         if to_json:
-            paths.append(os.path.join(loc, self._json_name))
+            paths.append(os.path.join(loc, self.json_name(save_name)))
             with open(paths[-1], "w", encoding="utf-8") as f:
                 # Save json. This does not guarantee writing to disk, so flushing
                 # and synchronization is also done to increase chance of writing
-                dump = rapidjson.dumps(to_json, indent=self._indent)
+                dump = rapidjson.dumps(to_json, indent=indent)
                 f.write(dump)
                 f.flush()
                 os.fsync(f.fileno())
-        for key, data in to_pickle.items():
-            paths.append(os.path.join(loc, f"{key}.{self._pickle_ext}"))
+
+        if to_pickle:
+            paths.append(os.path.join(loc, self.pickle_name(save_name)))
             with open(paths[-1], "wb") as f:
-                pickle.dump(data, f)
-        for seri, datas in func_serialize.items():
-            save, _, ext = SERIALIZATIONS[seri]
-            for key, data in datas.items():
-                paths.append(os.path.join(loc, f"{key}.{ext}"))
-                save(paths[-1], data)
+                pickle.dump(to_pickle, f)
+                f.flush()
+                os.fsync(f.fileno())
 
         return paths
 
     @classmethod
-    def load(cls, loc: str):
+    def load(cls, loc: str, save_name: Optional[str] = None):
         """
         Instantiates the DataStorage-inherited class by loading all files saved by `save` of that same class.
+        Use save_name to load json and pickle files that have been saved using explicitly set save_name.
         :param str loc: Path to directory from which to load data
         :return: An instance of this class with the content of the files
         """
 
-        fields = dict()
-        # List of fields non-loadable using the SERIALIZATIONS functions
-        generals = list()
+        json_file = os.path.join(loc, cls.json_name(save_name))
+        pickle_file = os.path.join(loc, cls.pickle_name(save_name))
 
-        for field_name in cls.__dict__["__dataclass_fields__"]:
-            for _, load, ext in SERIALIZATIONS.values():
-                datapath = os.path.join(loc, f"{field_name}.{ext}")
-                if os.path.exists(datapath):
-                    fields[field_name] = load(datapath)
-                    break
-            else:
-                generals.append(field_name)
-
-        # Check if the field was saved with pickle
-        any_json = False
-        for key in generals:
-            pfile = os.path.join(loc, f"{key}.{cls._pickle_ext}")
-            if os.path.isfile(pfile):
-                with open(pfile, "rb") as f:
-                    fields[key] = pickle.load(f)
-            else:
-                any_json = True
+        fields = dict()
 
-        if any_json:
-            with open(os.path.join(loc, cls._json_name), encoding="utf-8") as f:
+        if os.path.isfile(json_file):
+            with open(json_file, encoding="utf-8") as f:
                 fields.update(rapidjson.load(f))
 
+        if os.path.isfile(pickle_file):
+            with open(pickle_file, "rb") as f:
+                fields.update(pickle.load(f))
+
+        if not os.path.isfile(json_file) and not os.path.isfile(pickle_file):
+            raise FileNotFoundError("Unable to find saved %s files in directory %s with name %s" % (
+                cls.__name__, loc, (save_name or cls.__name__)
+            ))
+
         return cls(**fields)
```

### Comparing `pelutils-2.0.0/pelutils/ds/__init__.py` & `pelutils-3.0.0a1/pelutils/ds/__init__.py`

 * *Files identical despite different names*

### Comparing `pelutils-2.0.0/pelutils/ds/distributions.py` & `pelutils-3.0.0a1/pelutils/ds/distributions.py`

 * *Files identical despite different names*

### Comparing `pelutils-2.0.0/pelutils/ds/plots.py` & `pelutils-3.0.0a1/pelutils/ds/plots.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 import time
 from typing import Any, Callable, List, Optional, Union
 
 import numpy as np
 from . import _import_error
 try:
-    import matplotlib as mpl
     import matplotlib.pyplot as plt
     import matplotlib.colors as mcolour
     from scipy import stats
 except ModuleNotFoundError as e:
     raise _import_error from e
 
 
@@ -21,73 +20,82 @@
 base_colours: tuple[str] = tuple(mcolour.BASE_COLORS)
 # 10 colours
 tab_colours:  tuple[str] = tuple(mcolour.TABLEAU_COLORS)
 # 15 unique matplotlib colours
 colours:      tuple[str] = tab_colours[:-2] + base_colours[:-1]
 
 def moving_avg(
-    x: np.ndarray,
-    y: np.ndarray | None = None, *,
-    neighbors            = 3,
+    x: _Array,
+    y: Optional[_Array] = None, *,
+    neighbors               = 3,
 ) -> tuple[np.ndarray, np.ndarray]:
     """ Calculates the moving average assuming even spacing
     If one array of size n is given, it is assumed to run from 0 to n-1 on the x axis
     If two are given, the first are the x axis coordinates
-    Returns x and y coordinate arrays of same size """
+    Returns x and y coordinate arrays of same size. """
+    x = np.array(x)
     if y is None:
         y = x
         x = np.arange(x.size)
+    else:
+        y = np.array(y)
     x = x[neighbors:-neighbors]
     kernel = np.arange(1, 2*neighbors+2)
     kernel[-neighbors:] = np.arange(neighbors, 0, -1)
     kernel = kernel / kernel.sum()
     rolling = np.convolve(y, kernel, mode="valid")
     return x, rolling
 
 def exp_moving_avg(
-    x: np.ndarray,
-    y: np.ndarray | None = None, *,
-    alpha                = 0.2,
-    reverse              = False,
+    x: _Array,
+    y: Optional[_Array] = None, *,
+    alpha               = 0.2,
+    reverse             = False,
 ) -> np.ndarray:
     """ Calculates the exponential moving average
     alpha is a smoothing factor between 0 and 1 - the lower the value, the smoother the curve
     Returns two arrays of same size as x
-    This function optionally takes y as `moving_avg` """
+    This function optionally takes y as `moving_avg`. """
+    x = np.array(x)
     if y is None:
         y = x
         x = np.arange(x.size)
+    else:
+        y = np.array(y)
     if reverse:
         y = y[::-1]
 
     exp = np.empty(y.size)
     for i in range(y.size):
         if i:
             exp[i] = alpha * y[i] + (1 - alpha) * exp[i-1]
         else:
             exp[i] = y[i]
     return x, exp if not reverse else np.array(exp)[::-1]
 
 def double_moving_avg(
-    x: np.ndarray,
-    y: np.ndarray | None = None, *,
-    inner_neighbors      =   1,
-    outer_neighbors      =  12,
-    samples              = 300,
+    x: _Array,
+    y: Optional[_Array] = None, *,
+    inner_neighbors     =   1,
+    outer_neighbors     =  12,
+    samples             = 300,
 ) -> tuple[np.ndarray, np.ndarray]:
     """ Moving avg. function that produces smoother curves than normal moving avg.
     Also handles uneven data spacing better, and produces smoothed values for the entire span.
     This function optionally takes y as `moving_avg`.
     If both x and y are given, x must be sorted in ascending order.
     inner_neighbors: How many neighbors to use for the initial moving average.
     outer_neighbors: How many neighbors to use for for the second moving average.
     samples: How many points to sample the moving avg. at. """
+    x = np.array(x)
     if y is None:
         y = x
         x = np.arange(x.size)
+    else:
+        y = np.array(y)
     x = np.pad(x, pad_width=inner_neighbors)
     y = np.array([*[y[0]]*inner_neighbors, *y, *[y[-1]]*inner_neighbors])
     x, y = moving_avg(x, y, neighbors=inner_neighbors)
     # Sampled point along x axis
     extra_sample = outer_neighbors / samples
     # Sample points along x axis
     xx = np.linspace(
@@ -124,87 +132,73 @@
     """ Creates bins that fits nicely to a normally distributed variable
     Bins are smaller close to the mean of x """
     dist = stats.norm(np.mean(x), 3*np.std(x))
     p = min(dist.cdf(min(x)), 1-dist.cdf(max(x)))
     uniform_spacing = np.linspace(p, 1-p, bins)
     return dist.ppf(uniform_spacing)
 
-def get_bins(
+def histogram(
     data:         np.ndarray | list[float],
     binning_fn:   Callable[[_Array, int], _Array] = linear_binning,
     bins:         int  = 25,
     density:      bool = True,
     ignore_zeros: bool = False,
 ):
-    """ Create bins for plotting a line histogram. Simplest usage is plt.plot(*get_bins(data)) """
+    """ Create bins for plotting a line histogram. Simplest usage is plt.plot(*histogram(data)) """
     bins = np.array(binning_fn(data, bins+1))
     y, edges = np.histogram(data, bins=bins, density=density)
     x = (edges[1:] + edges[:-1]) / 2
     if ignore_zeros:
-        x, y = x[y>0], y[y>0]
+        keep = y > 0
+        x, y = x[keep], y[keep]
     return x, y
 
-def get_dateticks(x: _Array, num=7, date_format="%y-%m-%d") -> tuple[np.array, list[str]]:
+def get_dateticks(x: _Array, num=6, date_format="%b %d") -> tuple[np.ndarray, list[str]]:
     """ Produces date labels for the x axis given an array of epoch times in seconds. Simple usage:
     ```py
     # x is an array of epoch times in seconds
     plt.plot(x, y)
     plt.xticks(*get_dateticks(x))
     ``` """
     if not isinstance(num, int) or num < 2:
         raise ValueError("num must int of value 2 or greater, not %s" % num)
     x = np.array(x)
     xticks = np.linspace(x.min(), x.max(), num)
-    xticklabels = [time.strftime(date_format, time.gmtime(et)) for et in xticks]
+    xticklabels = [time.strftime(date_format, time.localtime(et)) for et in xticks]
     return xticks, xticklabels
 
 class Figure:
 
     """ Used for more ergonomic plotting. Simple usecase:
     ```py
     with Figure("figure.png", figsize=(20, 10), fontsize=50):
         plt.plot(x, y)
         plt.title("Very large title")
         plt.grid()
     # The finished figure is saved to "figure.png"
     # All settings are reset here
-    ```
-    It is also possible to access the figure and axis produced by plt.subplots.
-    These have type hinting, so it is for once possible to know what methods
-    and attributes exist on fig and ax.
-    In the example, the seaborn style is used (similar to `plt.style.use("seaborn"))`.
-    ```py
-    with Figure("figure.png", figsize=(20, 10), style="seaborn") as f:
-        f.ax.set_title("Normal sized title")
-        f.figure.add_axes(...)
     ``` """
 
     def __init__(
         self,
         savepath:     str, *,
-        # nrow and ncol are given to plt.subplots
-        # If either is larger than 1, the .ax attribute will be a numpy array
-        nrow:         int  = 1,
-        ncol:         int  = 1,
         tight_layout: bool = True,
         style:        Optional[str] = None,
         # Arguments below here go into mpl.rcParams
         figsize:           tuple[int, int] = (15, 10),
         dpi:               float = 200,
         fontsize:          float = 26,
         title_fontsize:    float = 0.5,   # Fraction of fontsize
         axes_ticksize:     float = 0.85,  # Fraction of fontsize
         legend_fontsize:   float = 0.85,  # Fraction of fontsize
         legend_framealpha: float = 0.8,
         legend_edgecolor:  tuple[float, float, float, float] = (0, 0, 0, 1),
         other_rc_params:   dict[str, Any] = dict(),
     ):
         self._savepath = savepath
-        self._nrow = nrow
-        self._ncol = ncol
         self._tight_layout = tight_layout
         self._style = style
 
         self._rc_params = {
             "font.size": fontsize,
             "figure.figsize": figsize,
             "figure.dpi": dpi,
@@ -220,26 +214,21 @@
     def __enter__(self):
         if self._style:
             plt.style.use(self._style)
 
         self._rc_context = plt.rc_context(self._rc_params)
         self._rc_context.__enter__()
 
-        self.fig, self.ax = plt.subplots(self._nrow, self._ncol)
-        self.fig: mpl.figure.Figure
-        self.ax: mpl.axes.Axes | np.ndarray
-
-        return self
-
     def __exit__(self, et, ev, tb):
         if self._tight_layout:
             plt.tight_layout()
         if not et:
             directory = os.path.split(self._savepath)[0]
             if directory:
                 os.makedirs(directory, exist_ok=True)
             plt.savefig(self._savepath)
+
         plt.close()
 
         self._rc_context.__exit__(et, ev, tb)
 
-        del self.fig, self.ax, self._rc_context
+        del self._rc_context
```

### Comparing `pelutils-2.0.0/pelutils/ds/stats.py` & `pelutils-3.0.0a1/pelutils/ds/stats.py`

 * *Files identical despite different names*

### Comparing `pelutils-2.0.0/pelutils/format.py` & `pelutils-3.0.0a1/pelutils/format.py`

 * *Files identical despite different names*

### Comparing `pelutils-2.0.0/pelutils/jsonl.py` & `pelutils-3.0.0a1/pelutils/jsonl.py`

 * *Files identical despite different names*

### Comparing `pelutils-2.0.0/pelutils/logging/__init__.py` & `pelutils-3.0.0a1/pelutils/logging/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,26 +107,26 @@
             return
         sep = sep or self._default_sep
         with_print = level >= self._print_level if with_print is None else with_print
         time = get_timestamp()
         tolog = sep.join([str(x) for x in tolog])
         time_spaces = len(time) * " "
         level_format = level.name + (self._maxlen - len(level.name)) * " "
-        space = self._spacing + self._maxlen * " " + self._spacing
+        space = self._spacing + self._maxlen * " " + self._spacing + " "
         logs = tolog.split("\n")
         rs = RichString()
         if with_info and tolog:
             rs.add_string(
-                f"{time}{self._spacing}{level_format}{self._spacing}",
+                f"{time}{self._spacing}{level_format}{self._spacing} ",
                 self._format(time, TIMESTAMP_COLOR) +\
                     self._spacing +\
                     self._format(level_format, LEVEL_FORMAT[level]) +\
                     self._spacing,
             )
-            rs.add_string(logs[0])
+            rs.add_string(logs[0].rstrip())
         else:
             rs.add_string(f"{time_spaces}{space}{logs[0]}".rstrip())
         for i in range(1, len(logs)):
             s = f"\n{time_spaces}{space}{logs[i]}".rstrip()
             rs.add_string(
                 s if s.strip() else "\n"
             )
```

### Comparing `pelutils-2.0.0/pelutils/logging/support.py` & `pelutils-3.0.0a1/pelutils/logging/support.py`

 * *Files identical despite different names*

### Comparing `pelutils-2.0.0/pelutils/parser.py` & `pelutils-3.0.0a1/pelutils/parser.py`

 * *Files identical despite different names*

### Comparing `pelutils-2.0.0/pelutils/tests.py` & `pelutils-3.0.0a1/pelutils/tests.py`

 * *Files identical despite different names*

### Comparing `pelutils-2.0.0/pelutils/ticktock.py` & `pelutils-3.0.0a1/pelutils/ticktock.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,17 +80,22 @@
     def __init__(self, tt, profile_name: str):
         self.tt = tt
         self.profile_name = profile_name
 
     def __enter__(self):
         pass
 
-    def __exit__(self, et, ev, tb):
+    def __exit__(self, et, _, __):
         if et == KeyboardInterrupt:
             return
+        if et is not None:
+            # If an exception occured in deeper profiling sections, make sure to end them
+            # before continuing, as a NameError otherwise will be raised due to unclosed profilings.
+            while self.tt._profile_stack[-1].name != self.profile_name:
+                self.tt.end_profile()
         self.tt.end_profile(self.profile_name)
 
 class TickTockException(RuntimeError):
     pass
 
 class TickTock:
     """ Simple time taker inspired by Matlab Tic, Toc, which also has profiling tooling.
@@ -159,15 +164,15 @@
     def profile(self, name: str, *, hits=1) -> _ProfileContext:
         """ Begin profile with given name. Optionally it is possible to
         register this as several hits that sum to the total time.
         This is usual when executing a multiprocessing mapping operation. """
         profile = Profile(
             name,
             len(self._profile_stack),
-            self._profile_stack[-1] if self._profile_stack else None
+            self._profile_stack[-1] if self._profile_stack else None,
         )
 
         if hash(profile) in self._id_to_profile:
             profile = self._id_to_profile[hash(profile)]
             if profile.parent is not None:
                 profile.parent.children.pop()
         else:
```

### Comparing `pelutils-2.0.0/pelutils.egg-info/PKG-INFO` & `pelutils-3.0.0a1/pelutils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelutils
-Version: 2.0.0
+Version: 3.0.0a1
 Summary: Utility functions that are often useful
 Home-page: https://github.com/peleiden/pelutils
 Author: Asger Laurits Schultz, Søren Winkel Holm
 Author-email: asger.s@protonmail.com, swholm@protonmail.com
 License: BSD-3-Clause
 Download-URL: https://pypi.org/project/pelutils/
 Keywords: utility,logger,parser,profiling,plotting
@@ -13,31 +13,31 @@
 Description-Content-Type: text/markdown
 Provides-Extra: ds
 Provides-Extra: tests
 License-File: pelutils/_c/hashmap.c/LICENSE
 
 # pelutils
 
+[![pytest](https://github.com/peleiden/pelutils/actions/workflows/pytest.yml/badge.svg?branch=master)](https://github.com/peleiden/pelutils/actions/workflows/pytest.yml)
+[![Coverage Status](https://coveralls.io/repos/github/peleiden/pelutils/badge.svg?branch=master)](https://coveralls.io/github/peleiden/pelutils?branch=master)
+
 Various utilities useful for Python projects. Features include
 
 - A simple and powerful logger with colourful printing and stacktrace logging
 - Parsing for combining config files and command-line arguments - especially useful for algorithms with several parameters
 - A timer inspired by Matlab's `tic` and `toc`
 - Simple code profiler
 - An extension to the built-in `dataclass` for saving and loading data
 - Table formatting
 - Miscellaneous standalone functions - see `pelutils/__init__.py`
 - Data-science submodule with extra utilities for statistics, plotting with `matplotlib`, and machine learning using `PyTorch`
 - Linear time `unique` function in the style of `numpy.unique`
 
 `pelutils` supports Python 3.7+.
 
-[![pytest](https://github.com/peleiden/pelutils/actions/workflows/pytest.yml/badge.svg?branch=master)](https://github.com/peleiden/pelutils/actions/workflows/pytest.yml)
-[![Coverage Status](https://coveralls.io/repos/github/peleiden/pelutils/badge.svg?branch=master)](https://coveralls.io/github/peleiden/pelutils?branch=master)
-
 ## Timing and Code Profiling
 
 Simple time taker inspired by Matlab Tic, Toc, which also has profiling tooling.
 
 ```py
 # Time a task
 TT.tick()
@@ -84,43 +84,33 @@
         tt2.tick()
     time.sleep(0.01)
 ```
 
 ## Data Storage
 
 The DataStorage class is an augmentation of the dataclass that incluces save and load functionality.
-This simplifies saving data, as only save command has to be issued for all data, and it keeps type hinting when loading data compared to e.g. a dictionary.
+This simplifies saving data, as only save command has to be issued for all data, and it keeps type
+hinting when loading data compared to e.g. a dictionary.
 
-Currently works specifically with:
-
-- Numpy arrays (`numpy.ndarray`)
-- Torch tensors (`torch.Tensor`)
-- Any `json` serializable data (as determined by the `rapidjson` library)
-
-All other data is pickled.
-
-DataStorage classes must inherit from DataStorage and be annotated with `@dataclass`.
-
-It is further possible to give arguments to the class definition:
-
-- `json_name`: Name of the saved json file
-- `indent`: How many spaces to use for indenting in the json file
+Data is in general preserved exactly as-is when saved data is loaded into memory with few exceptions.
+Notably, tuples are considered json-serializble, and so will be saved to the json file and will be
+loaded as lists.
 
 Usage example:
 
 ```py
 @dataclass
-class ResultData(DataStorage, json_name="game.json", indent=4):
+class ResultData(DataStorage):
     shots: int
     goalscorers: list
     dists: np.ndarray
 
 rdata = ResultData(shots=1, goalscorers=["Max Fenger"], dists=np.ones(22)*10)
 rdata.save("max")
-# Now shots and goalscorers are saved in <pwd>/max/game.json and dists in <pwd>/max/dists.npy
+# Now shots and goalscorers are saved in <pwd>/max/ResultData.json and dists in <pwd>/max/ResultData.pkl
 
 # Then to load
 rdata = ResultData.load("max")
 print(rdata.goalscorers)  # ["Max Fenger"]
 ```
 
 ## Parsing
@@ -260,15 +250,16 @@
 a, b = np.random.randn(100), np.random.randn(100)
 r, lower_r, upper_r, p = corr_ci(a, b, alpha=0.01)
 ```
 
 ## Plotting
 
 `pelutils` provides plotting utilities based on `matplotlib`.
-Most notable is the `Figure` context class, which attempts to remedy some of the common grievances with `matplotlib`, e.g. having to remember the correct `kwargs` and `rcParams` for setting font sizes, grid line colours etc, and notably adding type hinting to `fig` and `ax` produced by `plt.subplots`.
+Most notable is the `Figure` context class, which attempts to remedy some of the common grievances with `matplotlib`,
+e.g. having to remember the correct `kwargs` and `rcParams` for setting font sizes, legend edge colour etc.
 ```py
 from pelutils.ds.plots import Figure
 
 # The following makes a plot and saves it to `plot.png`.
 # The seaborn is style is used for demonstration, but if the `style` argument
 # is not given, the default matplotlib style is used.
 # The figure and font size are also given for demonstration, but their default
@@ -278,43 +269,35 @@
     plt.scatter(x, y, label="Data")
     plt.grid()
     plt.title("Very nice plot")
 # The figure is automatically saved to `plot.png` and closed, such that
 # plt.plot can be used again from here.
 # Figure changes `matplotlib.rcParams`, but these changes are also undone
 # after the end of the `with statement`.
-
-# For more complex plots, it is also possible to access the `fig` and `ax`
-# variables usually assigned as `fig, ax = plt.subplots()`.
-# These are type hinted, so no more remembering if it is `ax.title()` or
-# `ax.set_title()`.
-with Figure("plot.png") as f:
-    f.fig  # fig available as attribute on the Figure instance
-    f.ax.set_title("Very nice plot")  # The same goes for `ax`
 ```
 
 The plotting utilies also include binning functions for creating nice histograms.
-The `get_bins` function produces bins based on a binning function, of which three are provided:
+The `histogram` function produces bins based on a binning function, of which three are provided:
 
 - `linear_binning`: Bins are spaced evenly from the lowest to the largest value of the data.
 - `log_binning`: Bins are log-spaced from the lowest to the largest value of the data, which is assumed to be positive.
 - `normal_binning`: Bins are distributed according to the distribution of the data, such there are more bins closer to the center of the data. This is useful if the data somewhat resembles a normal distribution, as the resolution will be the greatest where there is the most data.
 
 It is also possible to provide custom binning functions.
 
-`get_bins` provide both `x` and `y` coordinates, making it simple to use with argument unpacking:
+`histogram` provide both `x` and `y` coordinates, making it simple to use with argument unpacking:
 ```py
 import matplotlib.pyplot as plt
 import numpy as np
-from pelutils.ds.plots import get_bins, normal_binning
+from pelutils.ds.plots import histogram, normal_binning
 
 # Generate normally distributed data
 x = np.random.randn(100)
 # Plot distribution
-plt.plot(*get_bins(x, binning_fn=normal_binning))
+plt.plot(*histogram(x, binning_fn=normal_binning))
 ```
 
 Finally, different smoothing functions are provided.
 The two most common are `moving_avg` and `exponential_avg` which smooth the data using a moving average and exponential smoothing, respectively.
 
 The `double_moving_avg` is special in that the number of smoothed data points do not depend on the number of given data points but is instead based on a given number of samples, which allows the resulting smoothed curve to not by jagged as happens with the other smoothing functions.
 It also has two smoothness parameters, which allows a large degree of smoothness control.
```

### Comparing `pelutils-2.0.0/pelutils.egg-info/SOURCES.txt` & `pelutils-3.0.0a1/pelutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pelutils-2.0.0/setup.py` & `pelutils-3.0.0a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 requirements_ds = [
     "torch>=1.7.0",
     "matplotlib>=3.1.0",
     "scipy>=1.4.1",
     "tqdm>=4.0.0",
 ]
 requirements_dev = [
-    "pytest>=6.2.4",
+    "pytest>=6.2.4,<=7.2",
     "pytest-cov>=2.12.1",
     "coveralls>=3.2.0",
     "coverage>=5.5",
     "wheel",
     "setuptools>=60.0.0",
 ]
```

