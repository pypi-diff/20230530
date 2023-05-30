# Comparing `tmp/equal-odds-0.0.6.tar.gz` & `tmp/equal-odds-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equal-odds-0.0.6.tar", last modified: Wed May 10 15:07:58 2023, max compression
+gzip compressed data, was "equal-odds-0.0.7.tar", last modified: Tue May 30 09:34:13 2023, max compression
```

## Comparing `equal-odds-0.0.6.tar` & `equal-odds-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:07:58.629537 equal-odds-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 15:07:45.000000 equal-odds-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 15:07:45.000000 equal-odds-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-10 15:07:58.629537 equal-odds-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-10 15:07:45.000000 equal-odds-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:07:58.625537 equal-odds-0.0.6/equal_odds/
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-05-10 15:07:45.000000 equal-odds-0.0.6/equal_odds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 15:07:45.000000 equal-odds-0.0.6/equal_odds/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16475 2023-05-10 15:07:45.000000 equal-odds-0.0.6/equal_odds/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-05-10 15:07:45.000000 equal-odds-0.0.6/equal_odds/cvxpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-05-10 15:07:45.000000 equal-odds-0.0.6/equal_odds/equal_odds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-10 15:07:45.000000 equal-odds-0.0.6/equal_odds/roc_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:07:58.625537 equal-odds-0.0.6/equal_odds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-10 15:07:58.000000 equal-odds-0.0.6/equal_odds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-10 15:07:58.000000 equal-odds-0.0.6/equal_odds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:07:58.000000 equal-odds-0.0.6/equal_odds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 15:07:58.000000 equal-odds-0.0.6/equal_odds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 15:07:58.000000 equal-odds-0.0.6/equal_odds.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:07:58.629537 equal-odds-0.0.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 15:07:45.000000 equal-odds-0.0.6/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 15:07:45.000000 equal-odds-0.0.6/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 15:07:45.000000 equal-odds-0.0.6/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:07:58.629537 equal-odds-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-10 15:07:45.000000 equal-odds-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:34:13.524550 equal-odds-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-30 09:34:02.000000 equal-odds-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 09:34:02.000000 equal-odds-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-30 09:34:13.524550 equal-odds-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-30 09:34:02.000000 equal-odds-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:34:13.520550 equal-odds-0.0.7/equal_odds/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-05-30 09:34:02.000000 equal-odds-0.0.7/equal_odds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-30 09:34:02.000000 equal-odds-0.0.7/equal_odds/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16475 2023-05-30 09:34:02.000000 equal-odds-0.0.7/equal_odds/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16449 2023-05-30 09:34:02.000000 equal-odds-0.0.7/equal_odds/cvxpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-05-30 09:34:02.000000 equal-odds-0.0.7/equal_odds/equal_odds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-30 09:34:02.000000 equal-odds-0.0.7/equal_odds/roc_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:34:13.524550 equal-odds-0.0.7/equal_odds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-30 09:34:13.000000 equal-odds-0.0.7/equal_odds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-30 09:34:13.000000 equal-odds-0.0.7/equal_odds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:34:13.000000 equal-odds-0.0.7/equal_odds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-30 09:34:13.000000 equal-odds-0.0.7/equal_odds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 09:34:13.000000 equal-odds-0.0.7/equal_odds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:34:13.524550 equal-odds-0.0.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 09:34:02.000000 equal-odds-0.0.7/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-30 09:34:02.000000 equal-odds-0.0.7/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 09:34:02.000000 equal-odds-0.0.7/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 09:34:13.524550 equal-odds-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-30 09:34:02.000000 equal-odds-0.0.7/setup.py
```

### Comparing `equal-odds-0.0.6/LICENSE` & `equal-odds-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `equal-odds-0.0.6/PKG-INFO` & `equal-odds-0.0.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 Metadata-Version: 2.1
 Name: equal-odds
-Version: 0.0.6
+Version: 0.0.7
 Summary: _PACKAGE UNDER CONSTRUCTION_
 Home-page: https://github.com/AndreFCruz/equal-odds
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
 License-File: LICENSE
 
 # equal-odds
-> This repository is under construction :construction:
 
 ![PyPI publishing status](https://github.com/AndreFCruz/equal-odds/actions/workflows/python-publish.yml/badge.svg)
 ![PyPI version](https://badgen.net/pypi/v/equal-odds)
 ![OSI license](https://badgen.net/pypi/license/equal-odds)
 ![Python compatibility](https://badgen.net/pypi/python/equal-odds)
 <!-- ![PyPI version](https://img.shields.io/pypi/v/equal-odds) -->
 <!-- ![OSI license](https://img.shields.io/pypi/l/equal-odds) -->
 <!-- ![Compatible python versions](https://img.shields.io/pypi/pyversions/equal-odds) -->
 
-A fast adjust
+Fast postprocessing of any score-based predictor to meet fairness criteria.
+
+The `equal-odds` package can achieve strict or relaxed fairness constraint fulfillment, 
+which can be useful to compare ML models at equal fairness levels.
+
 
 ## Installing
 
 Install package from [PyPI](https://pypi.org/project/equal-odds/):
 ```
 pip install equal-odds
 ```
 
 Or, for development, you can clone the repo and install from local sources:
 ```
 git clone https://github.com/AndreFCruz/equal-odds.git
 pip install ./equal-odds
 ```
 
+
 ## Getting started
 
 ```py
 # Given any trained model that outputs real-valued scores
 fair_clf = RelaxedEqualOdds(
     predictor=lambda X: model.predict_proba(X)[:, -1],   # for sklearn API
     # predictor=model,  # use this for a callable model
@@ -60,7 +66,32 @@
 # This will find the optimal _fair classifier_
 fair_clf.fit(X=X, y=y, group=group)
 
 # Now you can use `fair_clf` as any other classifier
 # You have to provide group information to compute fair predictions
 y_pred_test = fair_clf(X=X_test, group=group_test)
 ```
+
+
+## How it works
+
+Given a callable score-based predictor (i.e., `y_pred = predictor(X)`), and some `(X, Y, S)` data to fit, `RelaxedEqualOdds` will:
+1. Compute group-specific ROC curves and their convex hulls;
+2. Compute the `r`-relaxed optimal solution for the chosen fairness criterion (using [cvxpy](https://www.cvxpy.org));
+3. Find the set of group-specific binary classifiers that match the optimal solution found.
+    - each group-specific classifier is made up of (possibly randomized) group-specific thresholds over the given predictor;
+    - if a group's ROC point is in the interior of its ROC curve, partial randomization of its predictions may be necessary.
+
+
+## Implementation road-map
+
+We welcome community contributions for [cvxpy](https://www.cvxpy.org) implementations of other fairness constraints.
+
+Currently implemented fairness constraints:
+- [x] equality of odds [(Hardt et al., 2016)](https://proceedings.neurips.cc/paper/2016/file/9d2682367c3935defcb1f9e247a97c0d-Paper.pdf);
+  - i.e., equal group-specific TPR and FPR;
+<!--
+- [ ] equal opportunity;
+  - i.e., equal group-specific TPR;
+- [ ] demographic parity;
+  - i.e., equal group-specific predicted prevalence;
+-->
```

### Comparing `equal-odds-0.0.6/equal_odds/classifiers.py` & `equal-odds-0.0.7/equal_odds/classifiers.py`

 * *Files identical despite different names*

### Comparing `equal-odds-0.0.6/equal_odds/cvxpy_utils.py` & `equal-odds-0.0.7/equal_odds/cvxpy_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,14 +319,16 @@
     Returns
     -------
     (groupwise_roc_points, global_roc_point) : tuple[np.ndarray, np.ndarray]
         A pair tuple, (<1>, <2>), containing:
         1: an array with the group-wise ROC points for the solution.
         2: an array with the single global ROC point for the solution.
     """
+    raise NotImplementedError("Not currently implemented; the problem is not convex!")
+
     logging.warning("> compute_equal_odds_unfair_optimum :: USE WITH CARE!")
     n_groups = len(groupwise_roc_hulls)
     assert n_groups == len(group_sizes_label_neg) == len(group_sizes_label_pos)
 
     # Group-wise ROC points
     groupwise_roc_points_vars = [
         cp.Variable(shape=2, name=f"ROC point for group {i}", nonneg=True)
@@ -348,15 +350,15 @@
         cp.norm_inf(groupwise_roc_points_vars[i] - groupwise_roc_points_vars[j])
         for i, j in product(range(n_groups), range(n_groups))
         if i < j
     ]
 
     # Constraint: the minimum disparity must be above `tolerance`
     constraints.append(
-        cp.min(groupwise_disparities) >= fairness_tolerance
+        cp.minimum(*groupwise_disparities) >= fairness_tolerance
     )
 
     # Constraints for points in respective group-wise ROC curves
     for idx in range(n_groups):
         constraints += make_cvxpy_point_in_polygon_constraints(
             polygon_vertices=groupwise_roc_hulls[idx],
             cvxpy_point=groupwise_roc_points_vars[idx])
```

### Comparing `equal-odds-0.0.6/equal_odds/equal_odds.py` & `equal-odds-0.0.7/equal_odds/equal_odds.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,18 +10,15 @@
 import logging
 from itertools import product
 from typing import Callable
 
 import numpy as np
 from sklearn.metrics import roc_curve
 
-from .cvxpy_utils import (
-    compute_equal_odds_optimum,
-    compute_equal_odds_unfair_optimum,
-)
+from .cvxpy_utils import compute_equal_odds_optimum
 from .roc_utils import (
     roc_convex_hull,
     plot_polygon_edges,
     calc_cost_of_point,
 )
 from .classifiers import (
     Classifier,
@@ -38,15 +35,14 @@
     def __init__(
             self,
             predictor: Callable[[np.ndarray], np.ndarray],
             tolerance: float,
             false_pos_cost: float = 1.0,
             false_neg_cost: float = 1.0,
             max_roc_ticks: int = 1000,
-            optimize_for_unfairness: bool = False,
             seed: int = 42,
             # distance: str = 'max',    # TODO: add option to use l1 or linf distances
         ):
         """Initializes the relaxed equal odds wrapper.
 
         Parameters
         ----------
@@ -60,43 +56,26 @@
         false_pos_cost : float, optional
             The cost of a FALSE POSITIVE error, by default 1.0.
         false_neg_cost : float, optional
             The cost of a FALSE NEGATIVE error, by default 1.0.
         max_roc_ticks : int, optional
             The maximum number of ticks (points) in each group's ROC, when
             computing the optimal fair classifier, by default 1000.
-        optimize_for_unfairness : bool, optional
-            If `optimize_for_unfairness=True`, the specified tolerance will be
-            the minimum allowed disparity instead of the maximum allowed 
-            disparity.
-            This is useful to compute the entire fairness-accuracy frontier.
-            i.e., `tolerance=0.2 and optimize_for_unfairness` will find the 
-            classifier with highest accuracy given the constraint that 
-            disparity (distance to fairness) is above 0.2.
         seed : int
             A random seed used for reproducibility when producing randomized
             classifiers.
         """
         # Save arguments
         self.predictor = predictor
         self.tolerance = tolerance
         self.false_pos_cost = false_pos_cost
         self.false_neg_cost = false_neg_cost
         self.max_roc_ticks = max_roc_ticks
-        self.optimize_for_unfairness = optimize_for_unfairness
         self.seed = seed
 
-        if self.optimize_for_unfairness:
-            logging.warning(
-                "> `optimize_for_unfairness=True` :: "
-                "will optimize for highest accuracy given a minimum level "
-                "(`tolerance`) of disparity/unfairness. "
-                "USE WITH CARE!"
-            )
-
         # Initialize instance variables
         self._all_roc_data: dict = None
         self._all_roc_hulls: dict = None
         self._groupwise_roc_points: np.ndarray = None
         self._global_roc_point: np.ndarray = None
         self._global_prevalence: float = None
         self._realized_classifier: EnsembleGroupwiseClassifiers = None
@@ -256,36 +235,23 @@
 
             curr_roc_points = np.stack((group_fpr, group_tpr), axis=1)
             curr_roc_points = np.vstack((curr_roc_points, [1, 0]))  # Add point (1, 0) to ROC curve
 
             self._all_roc_hulls[g] = roc_convex_hull(curr_roc_points)
 
         # Find the group-wise optima that fulfill the fairness criteria
-        if self.optimize_for_unfairness:
-            logging.warning("RelaxedEqualOdds :: optimizing for unfairness (use with care!)")
-            self._groupwise_roc_points, self._global_roc_point = compute_equal_odds_unfair_optimum(
-                groupwise_roc_hulls=self._all_roc_hulls,
-                fairness_tolerance=self.tolerance,
-                group_sizes_label_pos=group_sizes_label_pos,
-                group_sizes_label_neg=group_sizes_label_neg,
-                global_prevalence=self._global_prevalence,
-                false_positive_cost=self.false_pos_cost,
-                false_negative_cost=self.false_neg_cost,
-            )
-
-        else:
-            self._groupwise_roc_points, self._global_roc_point = compute_equal_odds_optimum(
-                groupwise_roc_hulls=self._all_roc_hulls,
-                fairness_tolerance=self.tolerance,
-                group_sizes_label_pos=group_sizes_label_pos,
-                group_sizes_label_neg=group_sizes_label_neg,
-                global_prevalence=self._global_prevalence,
-                false_positive_cost=self.false_pos_cost,
-                false_negative_cost=self.false_neg_cost,
-            )
+        self._groupwise_roc_points, self._global_roc_point = compute_equal_odds_optimum(
+            groupwise_roc_hulls=self._all_roc_hulls,
+            fairness_tolerance=self.tolerance,
+            group_sizes_label_pos=group_sizes_label_pos,
+            group_sizes_label_neg=group_sizes_label_neg,
+            global_prevalence=self._global_prevalence,
+            false_positive_cost=self.false_pos_cost,
+            false_negative_cost=self.false_neg_cost,
+        )
 
         # Construct each group-specific classifier
         all_rand_clfs = {
             g: RandomizedClassifier.construct_at_target_ROC(
                 predictor=self.predictor,
                 roc_curve_data=self._all_roc_data[g],
                 target_roc_point=self._groupwise_roc_points[g],
@@ -332,37 +298,33 @@
             self,
             plot_roc_curves: bool = False,
             plot_roc_hulls: bool = True,
             plot_group_optima: bool = True,
             plot_group_triangulation: bool = True,
             plot_global_optimum: bool = True,
             plot_diagonal: bool = True,
+            plot_relaxation: bool = False,
             group_name_map: dict = None,
+            figure = None,
             **fig_kwargs,
         ):
         self._check_fit_status()
     
-        import seaborn as sns
         from matplotlib import pyplot as plt
+        from matplotlib.patches import Rectangle
+        import seaborn as sns
 
         n_groups = len(self._all_roc_hulls)
 
         # Set group-wise colors and global color
         palette = sns.color_palette(n_colors=n_groups + 1)
         global_color = palette[0]
         all_group_colors = palette[1:]
 
-        fig = plt.figure(**fig_kwargs)
-
-        # Plot diagonal
-        if plot_diagonal:
-            plt.plot(
-                [0, 1], [0, 1],
-                ls='--', color="grey", alpha=0.5,
-            )
+        fig = figure if figure is not None else plt.figure(**fig_kwargs)
 
         # For each group `idx`
         for idx in range(n_groups):
             group_ls = (['--', ':', '-.'] * (1 + n_groups // 3))[idx]
             group_color = all_group_colors[idx]
 
             # Plot group-wise (actual) ROC curves
@@ -414,22 +376,54 @@
 
 
         # Plot global optimum
         if plot_global_optimum:
             plt.plot(
                 self._global_roc_point[0], self._global_roc_point[1],
                 label="global",
-                marker="^", color=global_color,
+                marker="*", color=global_color, alpha=0.6,
                 markersize=5, lw=0,
             )
 
-        plt.title(f"Solution to ({self.tolerance}-relaxed) equal odds optimum")
+        # Plot rectangle to visualize constraint relaxation
+        if plot_relaxation:
+
+            # Get rectangle points
+            min_x, max_x = np.min(self._groupwise_roc_points[:, 0]), np.max(self._groupwise_roc_points[:, 0])
+            min_y, max_y = np.min(self._groupwise_roc_points[:, 1]), np.max(self._groupwise_roc_points[:, 1])
+
+            # Draw relaxation rectangle
+            rect = Rectangle(
+                xy=(min_x, min_y),
+                width=max_x - min_x,
+                height=max_y - min_y,
+                facecolor="grey",
+                alpha=0.3,
+                label="relaxation",
+            )
+
+            # Add the patch to the Axes
+            ax = plt.gca()
+            ax.add_patch(rect)
+
+        # Plot diagonal
+        if plot_diagonal:
+            plt.plot(
+                [0, 1], [0, 1],
+                ls='--', color="grey", alpha=0.5,
+                label="random clf.",
+            )
+
+        # Set axis settings
+        plt.title(f"Solution to {self.tolerance}-relaxed equal odds optimum")
+        plt.xlabel("False Positive Rate")
+        plt.ylabel("True Positive Rate")
 
-        # TODO: construct a better legend; separating colors (per group) and markers (per function)
         plt.legend(loc="lower right", borderaxespad=2)
+
         # plt.show()
 
     def __call__(self, X: np.ndarray, group: np.ndarray) -> int:
         return self._realized_classifier(X, group)
 
     def predict(self, X: np.ndarray, group: np.ndarray) -> int:
         return self(X, group)
```

### Comparing `equal-odds-0.0.6/equal_odds/roc_utils.py` & `equal-odds-0.0.7/equal_odds/roc_utils.py`

 * *Files identical despite different names*

### Comparing `equal-odds-0.0.6/equal_odds.egg-info/PKG-INFO` & `equal-odds-0.0.7/equal_odds.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 Metadata-Version: 2.1
 Name: equal-odds
-Version: 0.0.6
+Version: 0.0.7
 Summary: _PACKAGE UNDER CONSTRUCTION_
 Home-page: https://github.com/AndreFCruz/equal-odds
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
 License-File: LICENSE
 
 # equal-odds
-> This repository is under construction :construction:
 
 ![PyPI publishing status](https://github.com/AndreFCruz/equal-odds/actions/workflows/python-publish.yml/badge.svg)
 ![PyPI version](https://badgen.net/pypi/v/equal-odds)
 ![OSI license](https://badgen.net/pypi/license/equal-odds)
 ![Python compatibility](https://badgen.net/pypi/python/equal-odds)
 <!-- ![PyPI version](https://img.shields.io/pypi/v/equal-odds) -->
 <!-- ![OSI license](https://img.shields.io/pypi/l/equal-odds) -->
 <!-- ![Compatible python versions](https://img.shields.io/pypi/pyversions/equal-odds) -->
 
-A fast adjust
+Fast postprocessing of any score-based predictor to meet fairness criteria.
+
+The `equal-odds` package can achieve strict or relaxed fairness constraint fulfillment, 
+which can be useful to compare ML models at equal fairness levels.
+
 
 ## Installing
 
 Install package from [PyPI](https://pypi.org/project/equal-odds/):
 ```
 pip install equal-odds
 ```
 
 Or, for development, you can clone the repo and install from local sources:
 ```
 git clone https://github.com/AndreFCruz/equal-odds.git
 pip install ./equal-odds
 ```
 
+
 ## Getting started
 
 ```py
 # Given any trained model that outputs real-valued scores
 fair_clf = RelaxedEqualOdds(
     predictor=lambda X: model.predict_proba(X)[:, -1],   # for sklearn API
     # predictor=model,  # use this for a callable model
@@ -60,7 +66,32 @@
 # This will find the optimal _fair classifier_
 fair_clf.fit(X=X, y=y, group=group)
 
 # Now you can use `fair_clf` as any other classifier
 # You have to provide group information to compute fair predictions
 y_pred_test = fair_clf(X=X_test, group=group_test)
 ```
+
+
+## How it works
+
+Given a callable score-based predictor (i.e., `y_pred = predictor(X)`), and some `(X, Y, S)` data to fit, `RelaxedEqualOdds` will:
+1. Compute group-specific ROC curves and their convex hulls;
+2. Compute the `r`-relaxed optimal solution for the chosen fairness criterion (using [cvxpy](https://www.cvxpy.org));
+3. Find the set of group-specific binary classifiers that match the optimal solution found.
+    - each group-specific classifier is made up of (possibly randomized) group-specific thresholds over the given predictor;
+    - if a group's ROC point is in the interior of its ROC curve, partial randomization of its predictions may be necessary.
+
+
+## Implementation road-map
+
+We welcome community contributions for [cvxpy](https://www.cvxpy.org) implementations of other fairness constraints.
+
+Currently implemented fairness constraints:
+- [x] equality of odds [(Hardt et al., 2016)](https://proceedings.neurips.cc/paper/2016/file/9d2682367c3935defcb1f9e247a97c0d-Paper.pdf);
+  - i.e., equal group-specific TPR and FPR;
+<!--
+- [ ] equal opportunity;
+  - i.e., equal group-specific TPR;
+- [ ] demographic parity;
+  - i.e., equal group-specific predicted prevalence;
+-->
```

### Comparing `equal-odds-0.0.6/setup.py` & `equal-odds-0.0.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -37,14 +37,20 @@
 
 ROOT_PATH = Path(__file__).parent
 README_PATH = ROOT_PATH / 'README.md'
 
 REQUIREMENTS_PATH = ROOT_PATH / 'requirements' / 'main.txt'
 requirements = load_requirements(REQUIREMENTS_PATH)
 
+DEV_REQUIREMENTS_PATH = ROOT_PATH / 'requirements' / 'dev.txt'
+dev_requirements = load_requirements(DEV_REQUIREMENTS_PATH)
+
+TEST_REQUIREMENTS_PATH = ROOT_PATH / 'requirements' / 'test.txt'
+test_requirements = load_requirements(TEST_REQUIREMENTS_PATH)
+
 
 # ---------------------------------------------------------------------------- #
 #                                   Version                                    #
 # ---------------------------------------------------------------------------- #
 SRC_PATH = ROOT_PATH / 'equal_odds'
 VERSION_PATH = SRC_PATH / '_version.py'
 
@@ -66,22 +72,26 @@
     long_description_content_type='text/markdown',
 
     python_requires='>=3.8',
 
     packages=find_packages(),    
     install_requires=requirements,
 
+    extras_require={
+        "test": dev_requirements,
+        "dev": test_requirements,
+    },
+
     author='AndreFCruz',
     url='https://github.com/AndreFCruz/equal-odds',
 
     license='MIT',
 
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        # 'Development Status :: 3 - Alpha',
+        'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

